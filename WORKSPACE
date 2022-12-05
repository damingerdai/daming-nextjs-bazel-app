workspace(
    name = "daming-nextjs-bazel-app",
    managed_directories = {"@npm": ["node_modules"]},
)

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
http_archive(
    name = "build_bazel_rules_nodejs",
    sha256 = "0e8a818724c0d5dcc10c31f9452ebd54b2ab94c452d4dcbb0d45a6636d2d5a44",
    urls = [
        "https://github.com/bazelbuild/rules_nodejs/releases/download/5.7.2/rules_nodejs-5.7.2.tar.gz",
        "https://ghproxy.com/https://github.com/bazelbuild/rules_nodejs/releases/download/5.7.2/rules_nodejs-5.7.2.tar.gz"
    ],
)

load("@build_bazel_rules_nodejs//:repositories.bzl", "build_bazel_rules_nodejs_dependencies")

build_bazel_rules_nodejs_dependencies()

load("@build_bazel_rules_nodejs//:index.bzl", "node_repositories")
node_repositories()

load("@build_bazel_rules_nodejs//:index.bzl", "yarn_install")


yarn_install(
    name = "npm",
    package_json = "//:package.json",
    yarn_lock = "//:yarn.lock",
)