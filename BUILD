# Library
cc_library(
	name = "shared",
	hdrs = ["shared.h"],
	deps = ["@abseil-cpp//absl/strings"],
	srcs = ["shared.cc"],
)

# Main program
cc_binary(
	name = "main",
	srcs = ["main.cc"],
	deps = [":shared"],
)

# Library tests
cc_test(
	name = "tests",
	srcs = ["tests.cc"],
	deps = [
	    ":shared",
			"@googletest//:gtest",
			"@googletest//:gtest_main",
	],
)
