package(default_visibility = ["//tensorboard:internal"])

load("//tensorboard/defs:defs.bzl", "tensorboard_webcomponent_library")
load("//tensorboard/defs:web.bzl", "ts_web_library")

licenses(["notice"])  # Apache 2.0

ts_web_library(
    name = "tf_graph_loader",
    srcs = ["tf-graph-loader.html"],
    path = "/tf-graph-loader",
    deps = [
        "//tensorboard/plugins/graphs/tf_graph_common",
        "//tensorboard/components/tf_imports:polymer",
    ],
)

tensorboard_webcomponent_library(
    name = "legacy",
    srcs = [":tf_graph_loader"],
    destdir = "tf-graph-loader",
    deps = [
        "//tensorboard/plugins/graphs/tf_graph_common:legacy",
        "//third_party/javascript/polymer/v1/polymer:lib",
    ],
)

