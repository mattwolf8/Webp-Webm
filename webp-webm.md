Batch convert PNG's in a folder to webP

$ `for file in images/*; do cwebp -q 50 "$file" -o "${file%.*}.webp"; done`


Convert a single PNG to webP
$ cwebp -q 50 image-bg@2x.jpg -o image-bg@2x.webp


Convert a folder of gifs into animated webp 
$ for file in gif/*; do gif2webp -q 40 "$file" -o "${file%.*}.webp"; done

