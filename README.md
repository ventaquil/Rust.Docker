# Rust Docker

## How to start?

1. Install Docker ([more here](https://docs.docker.com/engine/installation/)).
2. Clone this repository.
3. Put your code in `application` directory.
4. Use `docker-cargo` script as default `cargo` function.

## How it works?

When you use `docker-cargo` in the background Docker downloads latest Rust image.

You can simply modify `docker-cargo` to specify tag and work on version which you want.

After pull Docker starts a container, run your code and that's it. You don't need to install Rust locally - only Docker is needed.

## FAQ

1. Where put a code?

   Whole your code put in `application` directory.

2. My script isn't working!

   Enter into your repository in termial.
   After that just call `./docker-cargo`.

   **Tip** If you want to call script globally put it in `~/bin`.

3. Where can I find binary?

   First you need to call `docker-cargo build` (or `docker-cargo build --release`).
   Now look at directories in `application/target`.
   In one of these (`debug` or `release`) you can find your binary.
