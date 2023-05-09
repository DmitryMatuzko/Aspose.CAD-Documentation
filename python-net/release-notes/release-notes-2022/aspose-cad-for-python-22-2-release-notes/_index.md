---
title: "Aspose.CAD for Python 22.2 Release Notes"
type: docs
url: /python-net/aspose-cad-for-python-22-2-release-notes/
weight: 10
---

{{% alert color="primary" %}}

This page contains release notes for Aspose.CAD for Python 22.2.

{{% /alert %}}

{{% alert color="primary" %}}
Please welcome our brand new product, Aspose.CAD for Python 22.2! Aspose.CAD for Python is the unique solution on the market that makes possible exporting reports and operate CAD and BIM drawing files from Python to various image file formats.

The export formats currently include: PDF, WMF, SVG, EMF, BMP, GIF, JPG, JPEG, DICOM, WEBP, JP2, JPEG2000, PNG, TIFF, PSD, HTML5.
{{% /alert %}}

## Features

The first release of the product supports the following features:

- Easy and Lightweight Deployment - Aspose.CAD for Python is written purely in Java and is provided as a single JAR file that can easily be deployed on the machines running Python.
- High Fidelity to Report Design - Aspose.CAD for Python exports reports in such a way that they look identical to reports exported by the built-in exporters of Python.
- Multipage export -  Aspose.CAD for Python supports multipage export to the following formats:  Gif,  Tiff, Pdf.
- Batch export - Aspose.CAD for Python supports export reports from Python in batch mode. Each page of the report will be saved as a separate file.

## Usage Examples

{{< highlight python >}}

import aspose.cad as cad

cadImage = cad.image.load("drawing.dxf");

rasterizationOptions = cad.CadRasterizationOptions();
pdfOptions = cad.PdfOptions();

cadImage.Save("output.pdf", pdfOptions);

{{< /highlight >}}
