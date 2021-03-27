load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository", "new_git_repository")

http_archive(
    name = "googletest",
    sha256 = "1d547f2b83e16eed4f6e3d5504dab0be60886bcb19cc4c62ee174d3c2cca03a8",
    strip_prefix = "googletest-7aca84427f224eeed3144123d5230d5871e93347",
    urls = ["https://github.com/google/googletest/archive/7aca84427f224eeed3144123d5230d5871e93347.zip"],
)

bind(
    name = "gtest",
    actual = "@googletest//:gtest",
)

bind(
    name = "gtest_main",
    actual = "@googletest//:gtest_main",
)

git_repository(
    name = "com_github_gflags_gflags",
    remote = "https://github.com/gflags/gflags.git",
    tag = "v2.2.1",
)

http_archive(
    name = "google_glog",
    sha256 = "cbba86b5a63063999e0fc86de620a3ad22d6fd2aa5948bff4995dcd851074a0b",
    strip_prefix = "glog-c8f8135a5720aee7de8328b42e4c43f8aa2e60aa",
    urls = ["https://github.com/google/glog/archive/c8f8135a5720aee7de8328b42e4c43f8aa2e60aa.zip"],
)

bind(
    name = "glog",
    actual = "@google_glog//:glog"
    )

http_archive(
    name = "com_google_absl",
    # head as of 20210212
    sha256 = "5ec35586b685eea11f198bb6e75f870e37fde62d15b95a3897c37b2d0bbd9017",
    strip_prefix = "abseil-cpp-143a27800eb35f4568b9be51647726281916aac9",
    urls = ["https://github.com/abseil/abseil-cpp/archive/143a27800eb35f4568b9be51647726281916aac9.zip"],
)
