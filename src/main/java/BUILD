java_binary(
    name = "java-bin",
    main_class = "does.not.exist",
    visibility = ["//:__pkg__"],
    runtime_deps = [":servlets"],
)

java_library(
    name = "servlets",
    srcs = glob(["**/*.java"]),
    visibility = ["//src/test/java/com/google/devtools/dash:__pkg__"],
    deps = [
        "@com_google_appengine_java//:api",
        "@io_bazel//third_party:apache_velocity",
        "@io_bazel//third_party:guava",
        "@io_bazel_rules_appengine//appengine:javax.servlet.api",
        "//src/main/protobuf:proto_dash",
    ],
)
