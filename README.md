# Thesis template

Sample template to get you started with LaTeX thesis.

Fork this repository to bootstrap your thesis.

Source markdown files located at [src](src) directory.
Result is published at [publish](publish) directory.

Sample: [src/sample.tex](src/sample.tex)  
Preamble: [common/preamble.tex](common/preamble.tex)
Result: [publish/sample.pdf](publish/sample.pdf)

## Building

Following command builds your thesis into `.pdf`:

```
make
```

> Note: also converts [src/title.doc](src/title.doc) to pdf and prepends to the resulting artifact.

## Publishing

To "publish" the final `.pdf` you can use the following command which builds and copies `src/*.pdf` into `publish/*.pdf`
which can then be committed to the repo:

```
make publish
```
