py_library(
    name = "rbconfig",
    srcs = ["rbconfig.py"],
)

py_library(
    name = "rberror",
    srcs = ["rberror.py"],
)

py_library(
    name = "rbopt",
    srcs = ["rbopt.py"],
)

py_library(
    name = "rbuser",
    srcs = ["rbuser.py"],
)

py_library(
    name = "rbaccount",
    srcs = ["rbaccount.py"],
    deps = [
        ":rbconfig",
        ":rberror",
        ":rbopt",
        ":rbuser",
    ],
)

py_library(
    name = "rbuserdb",
    srcs = ["rbuserdb.py"],
    deps = [
        ":rberror",
        ":rbopt",
        ":rbuser",
    ],
)

py_binary(
    name = "useradm",
    srcs = ["useradm.py"],
    deps = [
        ":rbaccount",
        ":rbuserdb",
    ],
)
