# Description:
# TensorFlow is a computational framework, primarily for use in machine
# learning applications.

load("@rules_shell//shell:sh_binary.bzl", "sh_binary")

package(
    # copybara:uncomment default_applicable_licenses = ["//tensorflow:license"],
    licenses = ["notice"],
)

sh_binary(
    name = "parallel_gpu_execute",
    srcs = ["parallel_gpu_execute.sh"],
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
    visibility = ["//visibility:private"],
)
