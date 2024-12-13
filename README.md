# wasm-alert Example Project

This project demonstrates the use of the `wasm-alert` library to display WebAssembly-powered alerts in a web application. The project includes a simple HTML page, a JavaScript file that imports and uses the `wasm-alert` library, and a Webpack configuration for building and serving the application.

## Getting Started

To run this project, follow these steps:

1. Install Rust by going to the [Install Rust page](https://www.rust-lang.org/tools/install) and following the instructions. This installs a tool called "rustup", which lets you manage multiple versions of Rust. By default, it installs the latest stable Rust release, which you can use for general Rust development. Rustup installs rustc, the Rust compiler, cargo, Rust's package manager, rust-std, Rust's standard libraries, and some helpful docs — rust-docs.

2. Install wasm-pack by running the command `cargo install wasm-pack`.

3. Clone the repository to your local machine.

4. Navigate to the project directory in your terminal.

5. Run `wasm-pack build --target web` to compile the Rust code to WebAssembly and generate the JavaScript file that wraps up that WebAssembly file into a module the browser can understand.

6. Run `npm install` to install the project dependencies.

7. Run `npm run serve` to start the development server.

8. Open your web browser and navigate to `http://localhost:8080`.

## Project Structure

The project consists of the following directories and files:

* `index.html`: The HTML page that loads the JavaScript file and displays the alert.
* `index.js`: The JavaScript file that imports and uses the `wasm-alert` library.
* `package.json`: The project's package file, which lists dependencies and scripts.
* `webpack.config.js`: The Webpack configuration file for building and serving the application.
* `.gitignore`: A file that specifies directories and files to ignore in the Git repository.

## Dependencies

This project depends on the following packages:

* `wasm-alert`: A library for displaying WebAssembly-powered alerts.
* `copy-webpack-plugin`: A Webpack plugin for copying files during the build process.
* `webpack`, `webpack-cli`, and `webpack-dev-server`: Webpack and its CLI for building and serving the application.

## Build and Serve

To build the project, run `npm run build`. This will compile the JavaScript file and copy the HTML file to the `dist` directory.

To serve the project, run `npm run serve`. This will start the development server, which will rebuild the project on changes and serve it at `http://localhost:8080`.

## License

This project is licensed under the MIT License.
