# Rust Concurrent program following the Book Programming Rust --chapter2

## Mandelbort series image cretion using command line

Try to determine if `c` is in the Mandelbort set, using at most `limit` iterations to decide.

If `c` is not a member, return `i`, where `i` is the number of
iterations it took for `c` to leave the circle of radius 2 centered
the origin.

If `c` seems to be a member (more preciesely, if we reached the
iteration limie without being able to prove that `c` is not a member)
return `None`

If `c` is a proven a member, based on the `i` iterations numbers, color the pixel correspond to `c` on a grey scale. White is not a member and black is a member.

args:

- > FILE: output file name.
- > PIXELS: image dimensions (e.g. 4000x3000) single string
- > UPPERLEFT: upper left corner point in complex plain (e.g. -1.20,0.35)
- > LOWERRIGHT: lower right corner point in the complex plain (e.g. -1,0.20)

## run the program

```shell
cargo build --release
```

```shell
target/release/mandelbort FILE PIXELS UPPERLEFT LOWERRIGHT
```
