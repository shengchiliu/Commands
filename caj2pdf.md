# caj2pdf & img2pdf

## Install Dependencies

```sh
conda install -c conda-forge pypdf2
brew install mupdf-tools
```

## Usage

```sh
caj2pdf convert input.caj -o output.pdf     # caj to pdf
mutool convert -o output.pdf input.jpg      # jpg to pdf
```

Ref: 
- https://github.com/JeziL/caj2pdf
- https://superuser.com/questions/1182578/how-to-convert-pdf-to-grayscale-through-mutool-mupdf-tools
