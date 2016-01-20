load("@//tools/build_rules/go:def.bzl", "go_repositories")
go_repositories()

git_repository(
  name = "protobuf",
  remote = "https://github.com/google/protobuf",
  commit = "d5fb408",
)

bind(
  name = "protoc",
  actual = "@protobuf//:protoc"
)

new_git_repository(
  name = "go-protobuf",
  remote = "https://github.com/golang/protobuf",
  commit = "68415e7",
  build_file = "tools/custom_rules/BUILD.go-protobuf",
)

new_git_repository(
  name = "swift-protobuf",
  remote = "https://github.com/alexeyxo/protobuf-swift",
  commit = "7a5b4760b",
  build_file = "tools/custom_rules/BUILD.swift-protobuf",
)
