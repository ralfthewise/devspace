# Contribution Guidelines
Please read this guide if you plan to contribute to the DevSpace CLI. We welcome any kind of contribution. No matter if you are an experienced programmer or just starting, we are looking forward to your contribution.

## Reporting Issues
If you find a bug while working with the DevSpace CLI, please [open an issue on GitHub](https://github.com/devspace-cloud/devspace/issues/new?labels=kind%2Fbug&template=bug-report.md&title=Bug:) and let us know what went wrong. We will try to fix it as quickly as we can.

## Feature Requests
You are more than welcome to open issues in this project to [suggest new features](https://github.com/devspace-cloud/devspace/issues/new?labels=kind%2Ffeature&template=feature-request.md&title=Feature%20Request:).

## Contributing Code
This project is mainly written in Golang. To contribute code,
1. Ensure you are running golang version 1.11.4 or greater for go module support
2. Set the following environment variables:
    ```
    GO111MODULE=on
    GOFLAGS=-mod=vendor
    ```
3. Fork the project
4. Clone the project: `git clone https://github.com/[YOUR_USERNAME]/devspace && cd devspace`
5. Run `go clean -modcache`
6. Run `go mod vendor` to install the dependencies
7. Make changes to the code (add new dependencies to the Gopkg.toml)
8. Build the project, e.g. via `go build -o devspace.exe`
9. Make changes
10. Run tests: `go test ./...`
11. Format your code: `go fmt ./...`
12. Commit changes
13. Push commits
14. Open pull request

## Improving the Documentation
The documentation is contained within `./docs` and made with Docusaurus. See the [Docs README](./docs) for infos about developing the docs.
