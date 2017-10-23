# Description: Tensorflow Serving examples.

package(
    default_visibility = ["@tf_serving//tensorflow_serving:internal"],
    features = ["no_layering_check"],
)

licenses(["notice"])  # Apache 2.0

load("@tf_serving//tensorflow_serving:serving.bzl", "serving_proto_library")

filegroup(
    name = "all_files",
    srcs = glob(
        ["**/*"],
        exclude = [
            "**/METADATA",
            "**/OWNERS",
        ],
    ),
)

cc_binary(
    name = "greeter_server_cc",
    srcs = [
        "greeter_server.cc",
    ],
    deps = [
#        "@tf_serving//tensorflow_serving/apis:prediction_service_proto",
        "@grpc//:grpc++",
#        "@org_tensorflow//tensorflow/core:framework",
        "@protobuf//:protobuf_lite",
    ],
)
