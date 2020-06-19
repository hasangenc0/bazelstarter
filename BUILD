# Add rules here to build your software
# See https://docs.bazel.build/versions/master/build-ref.html#BUILD_files

package(default_visibility = ["//visibility:public"])

exports_files(["tsconfig.json"], visibility = ["//visibility:public"])

load("@npm_bazel_typescript//:index.bzl", "ts_library", "ts_setup_workspace")
ts_setup_workspace()

ts_library(
    name = "app",
    srcs = ["src/main.ts"],
    deps = ["//src/module"],
)
