# CRESCENT Earthquake Catalog Repository Book

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18636678.svg)](https://doi.org/10.5281/zenodo.18636678)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)

Documentation for the earthquake catalogs included in the CRESCENT Earthquake Catalog Viewer: a description of each catalog, metadata and formatting requirements, and instructions for submitting new catalogs.

**Read the book:** https://cascadiaquakes.github.io/earthquake_catalog_repository/

**Viewer:** https://eqcat.cascadiaquakes.org

---

## Contents

- **Introduction**: the repository and how catalogs are used in the viewer
- **Catalogs**: one page per catalog (`catalogs/`)
- **Submission Instructions**: catalog format, metadata requirements and how to submit (`submission.md`)

---

## Building Locally

The book is built with [MyST](https://mystmd.org). With Node.js installed, run from the repository root:

```bash
npx --yes mystmd start
```

Then open the URL it prints.

---

## Deployment

GitHub Actions builds the book on every push to `main` and publishes it to GitHub Pages.

---

## Contributing

1. Review the catalog structure and metadata requirements in the book.
2. Format your catalog according to the guidelines.
3. [Open an issue](https://github.com/cascadiaquakes/cascadia-earthquake-viewer/issues) on the viewer repository with your formatted catalog and description page.
4. Your contribution will be reviewed and, if approved, added to the repository and the viewer.

---

## How to Cite

Please cite the publication for each catalog you use, and the repository and viewer:

> Marfo, W., Thomas, A., Bachelot, L., Journeau, C., Ni, Y., Hirao, B., & Trugman, D. (2026). *The Cascadia Region Earthquake Science Center (CRESCENT) Earthquake Catalog Repository and Viewer* (v1.0.0). Zenodo. https://doi.org/10.5281/zenodo.18636678

```bibtex
@software{marfo2026crescent_eqcat_viewer,
  author    = {Marfo, William and Thomas, Amanda and Bachelot, Lo{\"i}c and Journeau, Cyril and Ni, Yiyu and Hirao, Brenton and Trugman, Daniel},
  title     = {{The Cascadia Region Earthquake Science Center (CRESCENT) Earthquake Catalog Repository and Viewer} (v1.0.0)},
  year      = {2026},
  version   = {1.0.0},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.18636678},
  url       = {https://doi.org/10.5281/zenodo.18636678}
}
```

---

## License

This project is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0). See [LICENSE](LICENSE).

---

## Contacts

- **William Marfo**, University of California, Davis: [wmarfo@ucdavis.edu](mailto:wmarfo@ucdavis.edu)
- **Amanda M. Thomas**, University of California, Davis: [amthom@ucdavis.edu](mailto:amthom@ucdavis.edu)
- **Loïc Bachelot**, University of Oregon: [lbachelo@uoregon.edu](mailto:lbachelo@uoregon.edu)

For corrections or suggestions, please [open an issue](https://github.com/cascadiaquakes/earthquake_catalog_repository/issues).

---

## Acknowledgments

<table>
  <tr>
    <td align="center" valign="middle">
      <img src="https://raw.githubusercontent.com/cascadiaquakes/.github/main/assets/crescent-circle.png" alt="CRESCENT Logo" width="150" />
    </td>
    <td align="center" valign="middle">
      <img src="https://raw.githubusercontent.com/cascadiaquakes/.github/main/assets/nsf-logo.png" alt="NSF Logo" width="450" />
    </td>
  </tr>
</table>

This project is supported by the National Science Foundation through the Cascadia Region Earthquake Science Center (CRESCENT), Cooperative Agreement EAR-2225286.
