load(
    "@io_bazel_rules_scala//scala:scala_import.bzl",
    "scala_import",
)
scala_import(
	name = "import",
	jars = ["@com_google_guava_guava//jar:file"]
)
java_library(
	name = "passing",
	deps = [":import"],
	srcs = ["Some.java"]
)
java_library(
	name = "transitive_user",
	deps = [":passing"],
	srcs = ["TransitiveUser.java"]
)