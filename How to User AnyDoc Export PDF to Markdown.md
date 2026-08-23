#anydoc #pdfmarkdown

mkdir -p ~/Documents/anydoc-output

anydoc "file" \
-o ~/Documents/anydoc-output/test1.md

ls -lh ~/anydoc-output


:
	anydoc '/home/nguyenvuquang/Downloads/luat cong doan 2024.pdf' -o ~/Documents/anydoc-output/luat-cong-doan-2024.md

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



