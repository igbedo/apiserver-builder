package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["integer_test.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/client-go/util/integer",
    library = ":go_default_library",
)

go_library(
    name = "go_default_library",
    srcs = ["integer.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/client-go/util/integer",
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
