# BitMapFilter

This program applies various filters to BMP images. It supports the following filters:

- Blur (b)
- Grayscale (g)
- Reflection (r)
- Sepia (s)

## Usage

To use the program, run the following command:

```bash
./filter [flag] infile outfile
```

Replace `[flag]` with the filter flag (e.g., `b` for blur, `g` for grayscale, etc.), `infile` with the input BMP file, and `outfile` with the output BMP file.

### Example

To blur an image named `input.bmp` and save the result as `output.bmp`, use the following command:

```bash
./filter b input.bmp output.bmp
```

## Requirements

- Standard C library (`stdio.h`, `stdlib.h`)
- `getopt.h` for command-line argument parsing
- `helpers.h` for image processing functions
- `math.h` for round function

## Building the Program

To build the program, compile using the Makefile:

```bash
make filter
```

## Notes

- The input image must be a 24-bit uncompressed BMP 4.0 file.
- Only one filter can be applied at a time.
