# Catalog Contribution Instructions

## Requirements

To contribute your earthquake catalog model to to the CRESCENT Earthquake Catalog Viewer please first make sure your catalog meets the following two requirements:

- **Study Area Requirement**: The majority (>50%) of events in the catalog must fall within the CRESCENT geographic footprint (latitude: 39° to 52°, longitude: -130° to -116°) or be completely contained in it.  If you publish a catalog that encompasses a larger region, you are welcome to submit a subset of the catalog that falls within this range.
- **Peer-reviewed**: All catalogss must be published in a peer-reviewed journal with an associated DOI.

If your earthquake catalog meets the requirements listed above please follow the steps in the catalog contribution section below.

(catalog-contrib)=
## Catalog Contribution

To contribute your catalog to the CRESCENT Earthquake Catalog Repository, please follow the steps below.

## Step 1: Prepare your catalog

Your catalog can be submitted as a comma-separated values (CSV) file with a single header row.  The header fields must be one of the following fields defined below.

### Required Fields:

- **LON:** Longitude
- **LAT:** Latitude
- **DEPTH:** Depth (km, positive downward)
- **YEAR**: Origin Time Year in GMT
- **MONTH**: Origin Time Month in GMT
- **DAY**: Origin Time Day in GMT
- **HOUR**: Origin Time Hour in GMT
- **MINUTE**: Origin Time Minute in GMT
- **SECOND**: Origin Time Second in GMT

### Optional Fields:

- **MAG:** Local Magnitude
- **STRIKE:** strike (degrees from North)
- **MAG:** dip (degrees from horizontal)
- **RAKE:** rake (Aki and Richards convention)
- **MAG:** moment (Nm)
- **M$_xx$:** Mxx (Nm) 
- **M_xy_:** Mxy (Nm)
- **M_xz_:** Mxy (Nm)
- **M_yy_:** Myy (Nm)
- **M_yz_:** Myz (Nm)
- **M_zz_:** Mzz (Nm)

Each row in the catalog should correspond to a different earthquake.

## Step 2: Prepare a Markdown file describing your catalog

Each earthquake catalog included in the CRESCENT Earthquake Catalog Repository has a corresponding page describing the catalog in the CRESCENT Earthquake Catalog Repository JupyterBook.  For example, the page describing the LFE catalog of Shelly et al. (2025) can be found <a href="https://cascadiaquakes.github.io/earthquake_catalog_repository/shelly-grl-2025/" target="_blank">here</a>.  

To create a JupyterBook page describing your catalog please use the following template.

:::{admonition} Catalog Markdown Template
:class: dropdown

```markdown
# {AuthorLastName} et al. ({Year})

## {Catalog / Paper Title}

{Author list}

[![DOI](https://img.shields.io/badge/DOI-{DOI_URL_ENCODED}-blue)](https://doi.org/{DOI})
In the DOI badge URL, replace `/` with `%2F` (URL encoding).


:::{figure} ./{figure_filename}.jpg
:label: fig:{short_label}

{Figure caption describing the catalog, region, time span, and key observations.}
::

## Abstract

{Abstract text describing the catalog and its scientific context.  Can be directly from the corresponding publication.}

## Catalog Summary

- **Region:** {Region name}  
- **Time span:** {YYYY–YYYY or YYYY-MM-DD to YYYY-MM-DD}  
- **Number of events:** {integer + event type}  
- **Detection Method:** {method, e.g. STA/LTA, ML}  
- **Association Method:** {method e.g. PyOcto, Manual}  
- **Location Method:** {method e.g. HypoInverse+HypoDD}  
- **Velocity Model:** {velocity model name + citation}  
:::

## Step 3: Submit your catalog to the repository

- **Submission Request**: Visit the <a href="https://github.com/cascadiaquakes/cascadia-earthquake-viewer/issues" target="_blank">CRESCENT Earthquake Catalog Viewer Issue Page</a> and create a submission request.
  - Your request must include a download link to the CSV file containing your catalog.  Attachments are not permitted.
  - Your request must include a download link to your markdown file containing your catalog description.  
  - Your request must include your contact information so we can get in touch if we have questions and notify you once your catalog is included in the viewer.

