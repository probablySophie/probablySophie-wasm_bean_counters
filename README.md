# Bean Counters - But make it WASM
 

Remaking the game [Bean Counters](https://clubpenguin.fandom.com/wiki/Bean_Counters) using [Rust WASM](https://www.rust-lang.org/what/wasm) and JavaScript, but not NodeJS.


#### Steps to Completion  
- [x] Get a box moving like the penguin does  
- [ ] Get objects flying from the right of the screen like they should  
- [ ] Catch them!!  
- [ ] Levels!  
- [ ] Text with the points & stuff  
- [ ] Make a penguin image  
- [ ] Get it to move nicely  
- [ ] Make more penguin images  
- [ ] Make the player object able to display different images / frames  
- [ ] Make images for the flying things
- [ ] Have them rotate slightly? (or change image to look like they're rotating?)
- [ ] A cute background
- [ ] Make it possible to choose the penguin's colour  


#### Dependencies

The Rust `wasm32` target.
```bash
rustup target add wasm32-unknown-unknown # This installs almost instantly
```

The `wasm` build thingamys we use
```bash
# This set of installs *may* slow down your computer for a little while
# While they're thinking about things
cargo install wasm-bindgen-cli
cargo install wasm-gc
cargo install wasm-opt
```

The Rust [http crate](https://crates.io/crates/https) that I'm using as a local test server
```bash
# There's something going on between the crate and Cargo that leads to this nightmare of an install command
RUSTC_BOOTSTRAP=1 cargo install --git https://github.com/thecoshman/http
```


#### Tutorials & Stuff

Things I used for this project

* [`joern-kaltz/webassembly-rust-snake`](https://github.com/joern-kalz/webassembly-rust-snake) *A truly amazing and incredibly simple demo.*  
* [Setting up WASM without NodeJS](https://dev.to/dandyvica/wasm-in-rust-without-nodejs-2e0c) *Everything you'll need to install for things to work*  
<!-- Look, I actually haven't really used these two all that much, so they're secret comment links
* [A simple WASM & Canvas explanation](https://rustwasm.github.io/wasm-bindgen/examples/2d-canvas.html) 
* [WASM bind-gen's paint example](https://rustwasm.github.io/wasm-bindgen/examples/paint.html)
-->
