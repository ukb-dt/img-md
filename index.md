```py
# Clean and improve OCR output readability
clean_text = pytesseract.image_to_string(image, lang="eng", config="--psm 4")

# Save as a markdown file
md_path = "/mnt/data/Middle_Ground_Article.md"
with open(md_path, "w", encoding="utf-8") as f:
    f.write(clean_text)

md_path
```
