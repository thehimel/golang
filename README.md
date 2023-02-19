# Go

## About

* [Read here](https://go.dev/doc/)

## Getting Started

### Install

* [Installation Guide](https://go.dev/doc/)
* Test installation: `go version`.

### IDE

* [Goland](https://www.jetbrains.com/go)

#### Settings

* Resolve import error
  * Settings | Go | Go Modules | ▢ Enable Go modules integration

### Hello, World!

* [hello.go](src/hello.go)

```bash
mkdir src
cd src
go mod init src/hello
touch hello.go  # Create the file
go mod tidy  # Add the new required modules and sums
go run .  # Run the file where main() is defined.
go run hello.go  # Run the file with file name. Useful when multiple declarations of main() present in the same module.
```

### Import External Packages

* Let us import [quote](https://pkg.go.dev/search?q=quote) package.
* Go to [https://pkg.go.dev](https://pkg.go.dev) and search for `quote`.
* [quote.go](src/quote.go)

```bash
touch quote.go
go mod tidy  # Add the new required modules and sums
go run quote.go
```

### Clea up Go Cache and Re-download

```bash
# The directory where the file "go.mod" is located
cd src

go clean --modcache && go mod download
go mod tidy 
```

## Useful Reads

* [How to Write Go Code](https://go.dev/doc/code)

## Sources

### Go Official Documentation

* https://go.dev/doc/
