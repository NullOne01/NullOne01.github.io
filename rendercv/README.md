# Tailored RenderCV resumes

Built from `reactive_resume.json` with RenderCV 2.8. Both versions preserve the source employment titles, contact details, education, and language levels; summaries, skill ordering, and experience bullets are tailored to each role. Hidden projects and empty sections are omitted. Updated for Nov 2026: compulsory military service (Nov 2025 – Nov 2026) was added to close the employment gap, the Eagle Dynamics end date was corrected to Nov 2025, and the MEng expected completion to Jun 2027.

From the repository root, regenerate the PDFs:

```sh
rendercv render rendercv/unity_gameplay_programmer.yaml --pdf-path ../output/pdf/unity_gameplay_programmer.pdf --output-folder /tmp/rendercv-unity --dont-generate-markdown --dont-generate-png
rendercv render rendercv/cpp_engine_programmer.yaml --pdf-path ../output/pdf/cpp_engine_programmer.pdf --output-folder /tmp/rendercv-cpp --dont-generate-markdown --dont-generate-png
```

The first render may download required Typst packages. PDFs are saved under `output/pdf/`; intermediate Typst files go to `/tmp/`.
