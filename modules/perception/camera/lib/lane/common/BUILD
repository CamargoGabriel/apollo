load("//tools:cpplint.bzl", "cpplint")
load("//tools:py_proto.bzl", "py_proto")

package(default_visibility = ["//visibility:public"])

cc_proto_library(
    name = "denseline_proto",
    deps = [
        ":denseline_proto_lib",
    ],
)

proto_library(
    name = "denseline_proto_lib",
    srcs = ["denseline.proto"],
)

cc_proto_library(
    name = "darkSCNN_proto",
    deps = [
        ":darkSCNN_proto_lib",
    ],
)

proto_library(
    name = "darkSCNN_proto_lib",
    srcs = ["darkSCNN.proto"],
)

cc_library(
    name = "common_functions",
    srcs = ["common_functions.cc"],
    hdrs = ["common_functions.h"],
    deps = [
        "//cyber",
        "//modules/perception/base",
        "@eigen",
    ],
)

py_proto(
    name = "darkSCNN_pb2",
    src = "darkSCNN.proto",
)

py_proto(
    name = "denseline_pb2",
    src = "denseline.proto",
)

cpplint()
