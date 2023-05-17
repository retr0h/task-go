# Task Go

A prescriptive Golang [Task][] runner.

## Prescriptivity

* Code linting by [golangci-lint][]
* [Ginkgo][] and [Gomega][] test framework
* Source formatting with [gofumpt][] and [golines][]
* Coverage report generated with [go-junit-report][]

## Install

Install [Task][]:

    $ brew install go-task

Install Taskfile into project:

    $ curl -o Taskfile.yml https://raw.githubusercontent.com/retr0h/task-go/main/Taskfile.yml
    $ task

## Usage

Install dependencies

    $ task deps

Module maintenance:

    $ task mod

Report likely mistakes in packages:

    $ task vet

Run Go's vulnerability scanner:

    $ task vuln

Compile and run Go program:

    $ task run

Test packages:

    $ task unit

Test all:

    $ task test

Auto format code:

    $ task fmt

Generate coverage:

    $ task cov

Reformat files whose formatting differs from `go_fmt_command`:

    $ task fmt

Check files whose formatting differs from `go_fmt_command`:

    $ task fmt:check

Generate markdown documentation for golang code:

    $ task doc:generate

List targets:

    $ task

## License

The [MIT] License.

[Task]: https://github.com/go-task/task
[golangci-lint]: https://golangci-lint.run/
[Ginkgo]: https://onsi.github.io/ginkgo/
[Gomega]: https://onsi.github.io/gomega/
[gofumpt]: https://pkg.go.dev/github.com/vearutop/gofumpt
[golines]: https://pkg.go.dev/github.com/wrype/golines
[go-junit-report]: https://pkg.go.dev/github.com/debspencer/go-junit-report
[MIT]: LICENSE
