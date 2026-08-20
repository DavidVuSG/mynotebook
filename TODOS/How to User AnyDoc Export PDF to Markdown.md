#anydoc #pdfmarkdown

mkdir -p ~/Documents/anydoc-output

anydoc "file" \
-o ~/Documents/anydoc-output/test1.md

ls -lh ~/anydoc-output


# Scan ORD

ocrmypdf -l vie+eng \
'/home/nguyenvuquang/Downloads/CamScanner 08-19-2026 21.27.pdf' \
~/Documents/anydoc-output/test1-ocr.pdf

anydoc \
~/Documents/anydoc-output/test1-ocr.pdf \
-o ~/Documents/anydoc-output/test1.md


ocrmypdf \
--force-ocr \
--deskew \
-l vie+eng \
'/home/nguyenvuquang/Downloads/CamScanner 08-19-2026 21.27.pdf' \
~/Documents/anydoc-output/test1-ocr.pdf



