load("//tensorflow:tensorflow.bzl", "py_strict_library")

package(
    licenses = ["notice"],  # Apache 2.0
)

filegroup(
    name = "all_files",
    srcs = glob(
        ["**/*"],
        exclude = [
            "**/METADATA",
            "**/OWNERS",
        ],
    ),
    visibility = ["//tensorflow:__subpackages__"],
)

py_strict_library(
    name = "autograph",
    srcs = [
        "__init__.py",
    ],
    srcs_version = "PY3",
    visibility = ["//visibility:public"],
    deps = [
        "//tensorflow/python:util",
        "//tensorflow/python/autograph/core",
        "//tensorflow/python/autograph/impl",
        "//tensorflow/python/autograph/lang",
        "//tensorflow/python/autograph/operators",
        "//tensorflow/python/autograph/utils",
    ],
)
