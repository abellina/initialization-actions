package(default_visibility = ["//visibility:public"])

py_test(
    name = "test_oozie",
    size = "enormous",
    srcs = ["test_oozie.py"],
    data = [
        "oozie.sh",
        "validate.sh",
        "verify_oozie_running.py",
    ],
    local = True,
    shard_count = 4,
    deps = [
        "//integration_tests:dataproc_test_case",
        "@io_abseil_py//absl/testing:parameterized",
    ],
)
