package(default_visibility = ["//tensorboard:internal"])

load("//tensorboard/defs:web.bzl", "ts_web_library")

licenses(["notice"])  # Apache 2.0

ts_web_library(
    name = "vz_distribution_chart",
    srcs = [
        "vz-distribution-chart.html",
        "vz-distribution-chart.ts",
    ],
    path = "/vz-distribution-chart",
    visibility = ["//visibility:public"],
    deps = [
        "//tensorboard/components/tf_imports:lodash",
        "//tensorboard/components/tf_imports:plottable",
        "//tensorboard/components/tf_imports:polymer",
        "//tensorboard/plugins/scalars/vz_line_chart",
    ],
)

ts_web_library(
    name = "demo",
    srcs = ["index.html"],
    path = "/vz-distribution-chart",
    deps = [
        ":vz_distribution_chart",
        "//tensorboard/components/tf_imports:webcomponentsjs",
        "@org_polymer_iron_demo_helpers",
        "@org_polymer_paper_styles",
    ],
)

