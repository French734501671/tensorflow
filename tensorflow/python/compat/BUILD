licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

load("//tensorflow:tensorflow.bzl", "tf_py_test")

py_library(
    name = "compat",
    srcs = ["compat.py"],
    srcs_version = "PY2AND3",
    visibility = ["//tensorflow:internal"],
)

tf_py_test(
    name = "compat_test",
    size = "small",
    srcs = ["compat_test.py"],
    additional_deps = [
        ":compat",
        "//tensorflow/python:client_testlib",
    ],
)
