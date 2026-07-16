# Certificate Images

Drop your certificate images in this folder using the **exact filenames** below.
The site already points to these paths — as soon as a matching file lands here,
that certification card will automatically show the real image on hover/tap
instead of the placeholder. No HTML edits needed.

| Certification                     | Required filename                          |
|------------------------------------|---------------------------------------------|
| AI in Healthcare (Edufabrica)      | `ai-in-healthcare.jpg`                       |
| Genetic Engineering (NPTEL)        | `genetic-engineering-nptel.jpg`              |
| Complex Biological Systems (NPTEL) | `complex-biological-systems-nptel.jpg`       |
| Linguaskill Business (Cambridge)   | `linguaskill-business-cambridge.jpg`         |
| PET (Cambridge)                    | `pet-cambridge.jpg`                          |

**Notes**
- `.jpg` is expected by default. If your file is `.png` or `.webp`, either
  rename it to `.jpg`, or open `index.html`, find the matching `<img src="assets/certs/...">`
  line, and update the extension.
- Recommended: compress images (e.g. via [tinypng.com](https://tinypng.com))
  before committing — keeps the repo light and the page fast.
- Recommended orientation: landscape, reasonably high resolution — the image
  is displayed with `object-fit: contain`, so it won't be cropped.
