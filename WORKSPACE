load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_foreign_cc",
    strip_prefix = "rules_foreign_cc-master",
    url = "https://github.com/bazelbuild/rules_foreign_cc/archive/master.zip",
)

load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

http_archive(
    name = "yasm",
    build_file = "@//:BUILD.yasm",
    strip_prefix = "yasm-1.3.0",
    urls = ["https://github.com/yasm/yasm/releases/download/v1.3.0/yasm-1.3.0.tar.gz"],
)
