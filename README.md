# Unidoc Image BUG

See https://github.com/unidoc/unipdf/issues/447

## Run

```bash
$ go run pdf_add_image_to_page.go blank.pdf -1 quince.jpg 0 0 320 output.pdf
```

## Results

```bash
$ ls -la
       4,911 Apr  2 16:44 blank.pdf
   1,561,519 Apr  2 16:30 quince.jpg
  18,745,526 Apr  2 16:59 output.pdf
```

`output.pdf` is much bigger than sum of `blank.pdf` + `quince.jpg`

