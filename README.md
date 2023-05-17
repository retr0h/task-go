# Task Go

A prescriptive Golang [Task][] runner.

## Prescriptivity

* Code linting by `golangci-lint`
* `Ginkgo` and `Gomega` test framework
* Source formatting with `gofumpt` and `golines`
* Coverage report generated with `go-junit-report`

## Install

Install [Task][]:

    $ brew install go-task

Install Taskfile into project:

    $ curl -o Taskfile.yml https://raw.githubusercontent.com/retr0h/task-go/main/Taskfile.yml
    $ task

## Usage

Install dependencies

    $ task go:deps

Module maintenance:

    $ task go:mod

Report likely mistakes in packages:

    $ task go:vet

Run Go's vulnerability scanner:

    $ task go:vuln

Compile and run Go program:

    $ task go:run

Test packages:

    $ task go:unit

Test all:

    $ task go:test

Auto format code:

    $ task go:fmt

Generate coverage:

    $ task go:cov

Reformat files whose formatting differs from `go_fmt_command`:

    $ task go:fmt

Check files whose formatting differs from `go_fmt_command`:

    $ task go:fmt:check

Generate markdown documentation for golang code:

    $ task go:doc:generate

List targets:

    $ task

## License

The [MIT] License.

[MIT]: LICENSE
[Task]: https://github.com/go-task/task
