# Compress final pdf
`ghostscript -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/printer -dNOPAUSE -dQUIET -dBATCH -sOutputFile=output.pdf input.pdf`

# Compress a png as jpeg and resize
`convert in.png -sampling-factor 4:2:0 -strip -quality 85 -interlace JPEG -colorspace RGB -resize 50% -background white -flatten out.jpg`
