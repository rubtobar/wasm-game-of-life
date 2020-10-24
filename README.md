<div align="center">

  <h1><code>Conway's Game of Life</code></h1>

  <strong>npm package as a kick start for Rust and WebAssembly</strong>

  <h3>
    <a href="https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life">What is Conway's game of life</a>
    <span> | </span>
    <a href="https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life">npm package</a>
  </h3>

  <sub>Built with Rust 🦀 and WebAssembly 🕸 </sub>
</div>

## About

This project is based on the Rust tutorial to get the [hands on WebAssembly][tutorials] making a npm package.

What im trying to make is a npm package to display a Conway's game as a background in a web browser.
To this purpose I`m using Rust compiled to web assebly to get a really eficient implementation.

[tutorials]: https://rustwasm.github.io/docs/book/game-of-life/introduction.html

## 🚴 Usage

### 🛠️ Build with `wasm-pack build` in the root folder. It will create a pkg/ folder with the .wasm code and the .js and .ts files.

```
wasm-pack build
```

### 🔬 Test in Headless Browsers with `wasm-pack test`

```
wasm-pack test --headless --firefox
```

## 🔧 Tools used

* [`wasm-bindgen`](https://github.com/rustwasm/wasm-bindgen) for communicating
  between WebAssembly and JavaScript.
* [`console_error_panic_hook`](https://github.com/rustwasm/console_error_panic_hook)
  for logging panic messages to the developer console.
* [`wee_alloc`](https://github.com/rustwasm/wee_alloc), an allocator optimized
  for small code size.
