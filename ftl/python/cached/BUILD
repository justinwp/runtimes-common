package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_docker//python:image.bzl",
    "py_image",
)

py_binary(
    name = "python_cached",
    srcs = [
        "main.py",
        "//ftl/cached:cached_lib",
    ],
    data = ["//ftl:python_builder.par"],
    main = "main.py",
    deps = [
        "//ftl:ftl_lib",
        "@containerregistry",
    ],
)
