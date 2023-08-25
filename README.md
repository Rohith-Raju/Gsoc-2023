# Google Summer of Code 2022 - CNCF at Falco

## Project Title: Falco Playground: Web IDE for Security Rules with WebAssembly

Falco provides an intuitive and highly expressive rule language for configuring its powerful runtime security engine. However, the community still lacks an official and frictionless IDE solution for writing and testing Falco rules.

Since the last few releases, the Falco libraries increased the support for multiple architectures and platforms, and the integrated rules validator added a new output in machine-readable JSON format.

The idea for this project is to add WebAssembly as a new officially-supported compilation target for Falco by leveraging the Emscripten toolchain, and creating a new development environment for security rules in the form of a web single-page application by running Falco right inside the browser. The end result is envisioned to be similar to the Go Playground, but without the need of any backend.

The beauty of this idea is the opportunity of experiencing very different technologies of the cloud-native landscape all in a single project: low-level system code close to the Linux kernel, the fast-growing WebAssembly world, and frontend development for a web application. The feasibility of the project has already been assessed.

### Expected Outcome

The rules editor playground will dramatically benefit the learning curve and the development experience of security practitioners writing Falco rules, and will be the basis on which new educational content could be created for the community.

The web application code will likely live in its own standalone repository under the Falcosecurity organization.

A stretch goal would be to provide reusable groundwork for future integrations with other IDEs supporting WebAssembly, such as Visual Studio Code.

## Commits and Pull requests for this Project

To compile falco libs to wasm: [Support build for wasm - Libs](https://github.com/falcosecurity/libs/pull/1156)
To compile falco to wasm: [Suport build for wasm - Falco](https://github.com/falcosecurity/falco/pull/2663)
You can find the commits for the playground here: [falco playground](https://github.com/Rohith-Raju/falco-playground/commits/master)

## Falco Playground in Action

![falco playground](./images/nice.png)

![falco playground](./images/error.png)

![falco playground](./images/falco%20demo.gif)

## Addional Pull requests

1. [Support Memfd syscall](https://github.com/falcosecurity/libs/pull/1127)
2. [Support pidfd_getfd Syscall](https://github.com/falcosecurity/libs/pull/1145)
3. [Pidfd_open syscall](https://github.com/falcosecurity/libs/pull/1187)
4. [Parsers for memfd](https://github.com/falcosecurity/libs/pull/1162)
