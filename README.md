# Histopathology-Image-Tiling
tessellating tumor area in whole slide images (WSI) into square tiles

# What is QuPath?

QuPath is open source software for bioimage analysis.
QuPath is often used for digital pathology applications because it offers a powerful set of tools for working with whole slide images - but it can be applied to lots of other kinds of image as well.

## Tumor Area Annotation

First, I made two projects in Qupath for COAD and READ (TCGA Colorectal Cancer Diagnostic Slides in SVS format). then, all slides were manually reviewed and tumor areas were annotated and labeled as tumor. QuPath has several tools for circling the tumor regionin.

## What is TileExporter script?

Here the TileExporter script in QuPath provides options to help export all or part of an image as distinct (possibly overlapping) image tiles of a fixed size, at any resolution.
I have used this scripts in order to tessellate tumor area into square tiles of 512px×512px edge length, corresponding to 256 µm×256 µm at a resolution of 0.5 µmpx−1 (downsampled to 20× magnification) with an overlap of 50 pixels in JPG format.


Example:

![Screenshot (356)](https://user-images.githubusercontent.com/89701701/176489802-83c84965-4bd3-412e-b381-3ac8288f7701.png)


![Screenshot (15)](https://user-images.githubusercontent.com/89701701/176490196-7ddddc64-9718-43e0-aaec-96f60a09b47a.png)


## Requirements:
QuPath vesion 0.3.2

## Refrences:

Bankhead, P., Loughrey, M.B., Fernández, J.A. et al. QuPath: Open source software for digital pathology image analysis. Sci Rep 7, 16878 (2017). https://doi.org/10.1038/s41598-017-17204-5

https://qupath.readthedocs.io/en/stable/index.html
