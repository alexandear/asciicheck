# asciicheck [![Go Report Card](https://goreportcard.com/badge/github.com/tdakkota/asciicheck)](https://goreportcard.com/report/github.com/tdakkota/asciicheck)
Simple linter to check that your code does not contain non-ASCII identifiers

# Install
  
```
go get -u github.com/tdakkota/asciicheck
```

# Usage
asciicheck uses [`singlechecker`](https://pkg.go.dev/golang.org/x/tools/go/analysis/singlechecker) package to run:

```
asciicheck: checks that all code identifiers does not have non-ASCII symbols in the name

Usage: asciicheck [-flag] [package]


Flags:
  -V	print version and exit
  -all
    	no effect (deprecated)
  -c int
    	display offending line with this many lines of context (default -1)
  -cpuprofile string
    	write CPU profile to this file
  -debug string
    	debug flags, any subset of "fpstv"
  -fix
    	apply all suggested fixes
  -flags
    	print analyzer flags in JSON
  -json
    	emit JSON output
  -memprofile string
    	write memory profile to this file
  -source
    	no effect (deprecated)
  -tags string
    	no effect (deprecated)
  -trace string
    	write trace log to this file
  -v	no effect (deprecated)
```