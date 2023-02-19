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

# Create the file and add code to it.
touch hello.go

# Add the new required modules and sums
go mod tidy 

# Run the file in a generic way
go run .

# Run the file with file name
go run hello.go
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
