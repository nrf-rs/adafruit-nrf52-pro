# Board Support Package for the Adafruit Feather nRF52 Pro

This crate is a Board Support Package (BSP). It wraps the HAL crate
(`nrf52832-hal`) for the on-board nRF52832, and provides high level wrappers for
the onboard features.

## Usage

You will require the `thumbv7em-none-eabihf` target installed. To build one of these examples:

```console
$ rustup target add thumbv7em-none-eabihf
$ git clone https://github.com/nrf-rs/nrf-bsp-template.git
$ cd nrf-bsp-template
$ cargo build --target=thumbv7em-none-eabihf --example blinky
```

To use in your own application, add as a dependency and call the
`Board::take()` function.

## Minimum Supported Rust Version

This crate is guaranteed to build on stable Rust 1.41 and higher.

## Licence

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
  http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

## Contribution

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed as above, without any additional terms or
conditions.
