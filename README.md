
# eyedroppeR <img src='dev/images/hex1.png' align="right" height="240" />

`eyedroppeR` allows you to choose an image, plot it and click on the
image to return the hex codes of the selected pixel.

There are a few ways to get colours from an image but this aims is to
provide a simple, no fuss approach to get the hex codes into R.

## Installation

``` r
devtools::install_github("doehm/eyedroppeR")
```

## Usage

Use `eyedropper` with the following steps:

1.  Find the image you want to pick colours from online.

2.  Right-click and ‘copy image address’.

3.  Choose how many colours to pick e.g. `n = 5`.

4.  Run `pal <- eyedropper(n = 5)`. The function will read the copied
    address from the clipboard.

    4.a. If you have a local file or a saved `path` you can reference it
    directly with `pal <- eyedropper(n = 5, img_path = path)`

5.  Click 5 areas of the image (or however many you chose). The image
    will be stretched to the borders of the window, but that’s OK.

6.  Done! Copy the returned string and add it to you script and start
    using `pal`.
