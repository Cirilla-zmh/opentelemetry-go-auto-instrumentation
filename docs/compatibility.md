# Compatibility

OpenTelemetry-Go Contrib ensures compatibility with the current supported
versions of
the [Go language](https://golang.org/doc/devel/release#policy):

> Each major Go release is supported until there are two newer major releases.
> For example, Go 1.5 was supported until the Go 1.7 release, and Go 1.6 was supported until the Go 1.8 release.

For versions of Go that are no longer supported upstream, opentelemetry-go-contrib will
stop ensuring compatibility with these versions in the following manner:

- A minor release of opentelemetry-go-contrib will be made to add support for the new
  supported release of Go.
- The following minor release of opentelemetry-go-contrib will remove compatibility
  testing for the oldest (now archived upstream) version of Go. This, and
  future, releases of opentelemetry-go-contrib may include features only supported by
  the currently supported versions of Go.

This project is tested on the following systems.

| OS       | Go Version | Architecture |
| -------- | ---------- | ------------ |
| Ubuntu   | 1.22       | amd64        |
| Ubuntu   | 1.21       | amd64        |
| Ubuntu   | 1.22       | 386          |
| Ubuntu   | 1.21       | 386          |
| macOS 13 | 1.22       | amd64        |
| macOS 13 | 1.21       | amd64        |
| macOS    | 1.22       | arm64        |
| macOS    | 1.21       | arm64        |
| Windows  | 1.22       | amd64        |
| Windows  | 1.21       | amd64        |
| Windows  | 1.22       | 386          |
| Windows  | 1.21       | 386          |

While this project should work for other systems, no compatibility guarantees
are made for those systems currently.