# Copyright 2020 Google LLC
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

load(
    "//bazel:rules.bzl",
    "stratum_cc_library",
)

package(
    default_visibility = ["//visibility:public"],
    licenses = ["notice"],
)

stratum_cc_library(
    name = "sdn_controller_manager",
    srcs = ["sdn_controller_manager.cc"],
    hdrs = ["sdn_controller_manager.h"],
    deps = [
        "@com_github_google_glog//:glog",
        "@com_github_grpc_grpc//:grpc++",
        "@com_github_p4lang_p4runtime//:p4runtime_cc_grpc",
        "@com_github_p4lang_p4runtime//:p4runtime_cc_proto",
        "@com_google_absl//absl/container:flat_hash_map",
        "@com_google_absl//absl/numeric:int128",
        "@com_google_absl//absl/status",
        "@com_google_absl//absl/strings",
        "@com_google_absl//absl/strings:str_format",
    ],
)

stratum_cc_library(
    name = "stream_message_reader_writer_mock",
    testonly = 1,
    hdrs = ["stream_message_reader_writer_mock.h"],
    deps = [
        "@com_github_grpc_grpc//:grpc++",
        "@com_github_p4lang_p4runtime//:p4runtime_cc_proto",
        "@com_google_googletest//:gtest",
    ],
)
