load("//thrift:thrift.bzl", "thrift_library")
load("//twitter_scrooge:twitter_scrooge.bzl", "scrooge_scala_library")

thrift_library(
  name = "hello",
  srcs = ["Hello.thrift"],
  deps = ["//test/src/main/scala/scala/test/twitter_scrooge/canidep/Goodbye:goodbye"],
  visibility = ["//visibility:public"],
)

scrooge_scala_library(
  name = "canidep",
  deps = [
    ":hello",
  ],
  visibility = ["//visibility:public"],
)
