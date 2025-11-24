load("//pytype_bazel:pytype.bzl", "pytype_library")

pytype_library(
    name = "__init__",
    srcs = ["__init__.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":c4_trainer",
        ":common",
        ":deterministic_trainer",
        ":envy",
        ":fuji",
        ":gala",
        ":gala_sigmoid",
        ":gspmd",
        ":honeycrisp",
        ":pajama_sigmoid_trainer",
        ":pajama_trainer",
        ":vocabulary_fuji_v3",
    ],
)

pytype_library(
    name = "common",
    srcs = ["common.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        "//axlearn/common:attention",
        "//axlearn/common:causal_lm",
        "//axlearn/common:checkpointer",
        "//axlearn/common:config",
        "//axlearn/common:decoder",
        "//axlearn/common:embedding",
        "//axlearn/common:evaler",
        "//axlearn/common:input_dispatch",
        "//axlearn/common:input_fake",
        "//axlearn/common:input_lm",
        "//axlearn/common:input_tf_data",
        "//axlearn/common:layers",
        "//axlearn/common:learner",
        "//axlearn/common:mixture_of_experts",
        "//axlearn/common:optimizer_base",
        "//axlearn/common:param_init",
        "//axlearn/common:summary_writer",
        "//axlearn/common:trainer",
        "//axlearn/common:utils",
        "//axlearn/common/flash_attention:layer",
        "//axlearn/experiments/text:common",
        "@axlearn_pip//jax",
        "@axlearn_pip//tensorflow",
    ],
)

pytype_library(
    name = "c4_trainer",
    srcs = ["c4_trainer.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
        "//axlearn/experiments/text:common",
    ],
)

pytype_library(
    name = "deterministic_trainer",
    srcs = ["deterministic_trainer.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
        "//axlearn/experiments/text:common",
    ],
)

pytype_library(
    name = "pajama_sigmoid_trainer",
    srcs = ["pajama_sigmoid_trainer.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
        "//axlearn/experiments/text:common",
    ],
)

pytype_library(
    name = "pajama_trainer",
    srcs = ["pajama_trainer.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
        "//axlearn/experiments/text:common",
    ],
)

pytype_library(
    name = "envy",
    srcs = ["envy.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
    ],
)

pytype_library(
    name = "fuji",
    srcs = ["fuji.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
        "//axlearn/common:trainer_config_modifier",
    ],
)

pytype_library(
    name = "gala",
    srcs = ["gala.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
    ],
)

pytype_library(
    name = "gala_sigmoid",
    srcs = ["gala_sigmoid.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
    ],
)

pytype_library(
    name = "gspmd",
    srcs = ["gspmd.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
    ],
)

pytype_library(
    name = "honeycrisp",
    srcs = ["honeycrisp.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        ":common",
        "//axlearn/common:config",
    ],
)

pytype_library(
    name = "vocabulary_fuji_v3",
    srcs = ["vocabulary_fuji_v3.py"],
    enable_pytype = False,
    visibility = ["//visibility:public"],
    deps = [
        "//axlearn/common:config",
        "//axlearn/common:vocabulary_bpe",
    ],
)
