# Copyright 2016 The Closure Rules Authors. All rights reserved.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#    http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

package(default_visibility = ["//visibility:public"])

licenses(["notice"])  # Apache License 2.0

java_library(
    name = "soy",
    exports = ["@soy//jar"],
    runtime_deps = [
        "@aopalliance//jar",
        "@asm//jar",
        "@asm_analysis//jar",
        "@asm_commons//jar",
        "@asm_util//jar",
        "@gson//jar",
        "@guava//jar",
        "@guice//jar",
        "@guice_assistedinject//jar",
        "@guice_multibindings//jar",
        "@icu4j//jar",
        "@json//jar",
        "@jsr305//jar",
        "@jsr330_inject//jar",
        "@protobuf_java//jar",
        "@safe_html_types//jar",
    ],
)

java_binary(
    name = "SoyParseInfoGenerator",
    jvm_flags = ["-client"],
    main_class = "com.google.template.soy.SoyParseInfoGenerator",
    runtime_deps = [
        ":soy",
        "@args4j//jar",
    ],
)

java_binary(
    name = "SoyToJbcSrcCompiler",
    jvm_flags = ["-client"],
    main_class = "com.google.template.soy.SoyToJbcSrcCompiler",
    runtime_deps = [
        ":soy",
        "@args4j//jar",
    ],
)

java_binary(
    name = "SoyToJsSrcCompiler",
    jvm_flags = ["-client"],
    main_class = "com.google.template.soy.SoyToJsSrcCompiler",
    runtime_deps = [
        ":soy",
        "@args4j//jar",
    ],
)

java_binary(
    name = "SoyMsgExtractor",
    jvm_flags = ["-client"],
    main_class = "com.google.template.soy.SoyMsgExtractor",
    runtime_deps = [
        ":soy",
        "@args4j//jar",
    ],
)

java_binary(
    name = "SoyToPySrcCompiler",
    jvm_flags = ["-client"],
    main_class = "com.google.template.soy.SoyToPySrcCompiler",
    runtime_deps = [
        ":soy",
        "@args4j//jar",
    ],
)

java_binary(
    name = "SoyToIncrementalDomSrcCompiler",
    jvm_flags = ["-client"],
    main_class = "com.google.template.soy.SoyToIncrementalDomSrcCompiler",
    runtime_deps = [
        ":soy",
        "@args4j//jar",
    ],
)
