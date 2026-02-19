# Dissertation repository (GitHub-ready)

## Purpose
- **source/**: original files (DOCX, XLSX, etc.) kept for traceability.
- **llm/**: LLM-friendly versions:
  - `*.md` (text-first, with placeholders and links to compressed images)
  - `*_light.docx` (text-only DOCX without embedded images)
- **assets/**: extracted and compressed images:
  - `assets/img_original/<doc>/` (original extracted images)
  - `assets/img_webp/<doc>/` (compressed WEBP versions for GitHub/LLM workflows)

## Recommended workflow
1. Work with LLMs primarily on files in `llm/` (Markdown is best).
2. Keep editing in your preferred authoring format under `source/`.
3. When you update a source DOCX, re-run the same conversion pipeline to refresh `llm/` and `assets/`.

## GitHub tips
- If `source/` grows above ~50–100 MB, consider Git LFS for `.docx` and other binaries.
- Keep `llm/` and `assets/img_webp/` in normal Git (they stay small and diff-friendly enough).

## Entry point
Open: `llm/index.md`
