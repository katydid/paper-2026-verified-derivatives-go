## Verified Derivatives for Fast Filtering and Schema Validation of Semi-Structured Data (Golang)

[![Build Status](https://github.com/katydid/paper-2026-verified-filter-go/actions/workflows/build.yml/badge.svg)](https://github.com/katydid/paper-2026-verified-filter-go/actions)

The Go implementation of [Verified Derivatives for Fast Filtering and Schema Validation of Semi-Structured Data](http://katydid.org.za/paper-2026-verified-filter/).

How to run and reproduce the benchmarks:

1. Clone this repo into a folder that ends with `./src/github.com/katydid/paper-2026-verified-filter-go`
2. Clone https://github.com/katydid/paper-2026-verified-derivatives-testsuite into `./src/github.com/katydid/paper-2026-verified-filter-testsuite` relative to this repo
3. Install [Go](https://golang.org) version 1.24
4. Install protoc version 29.3 by [downloading](https://github.com/protocolbuffers/protobuf/releases/download/v29.3/protoc-29.3-linux-x86_64.zip) it from [Protobuf releases](https://github.com/protocolbuffers/protobuf/releases) and placing the `protoc` binary in your `PATH`.
5. Generate benchmarks by going to `./src/github.com/katydid/paper-2026-verified-filter-testsuite` and running `make regenerate-paper-benchmarks`. This can take a few minutes.
6. Go to `./src/github.com/katydid/paper-2026-verified-filter-go` and run `make paper_benchmarks`.

This repo was originally based on [katydid/validator-go-proto](https://github.com/katydid/validator-go-proto/commit/483e7705c19b9dd6afe9c084be08082c273d437b).
