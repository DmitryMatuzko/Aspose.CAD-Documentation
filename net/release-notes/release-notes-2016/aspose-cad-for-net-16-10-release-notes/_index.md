---
title: Aspose.CAD for .NET 16.10 Release notes
type: docs
weight: 30
url: /net/aspose-cad-for-net-16-10-release-notes/
---

Aspose.CAD for .Net has been updated to version 16.10 and we are pleased to announce it. The following is a list of changes in this version of Aspose.CAD.
### **Features and Improvements**

|**Key** |**Summary** |**Category** |
| :- | :- | :- |
|CADNET-134 |Integrate metering module to promote new sales model for Aspose.CAD |New Feature |
|CADNET-164 |[Loading DGN file is throwing exception](http://www.aspose.com/community/forums/thread/785056/aspose.cad-1.1.0-failed-to-load-dgn-file.aspx)|Enhancement |
|CADNET-156 |[Converting DWG to PNG format is producing very small PNG image that is unable to view](http://www.aspose.com/community/forums/thread/783250/aspose.cad-1.1.0-dwg-document-is-rendered-into-small-image.aspx)|Enhancement |
|CADNET-155 |Adjust Metered module quota consumption algorythm |Enhancement |
|CADNET-154 |Fix application menu URLs |Enhancement |
|CADNET-152 |[CAD Hatches Offsetting After Printing PDF](http://www.aspose.com/community/forums/thread/779909.aspx)|Enhancement |
|CADNET-149 |[Converting DXF to Image is working but producing shapes with very thin lines; not of proper width of lines](http://www.aspose.com/community/forums/thread/778925/cad-for-.net-line-thickness-problem-xl-64435.aspx)|Enhancement |
|CADNET-147 |Make Dgn exporter respects '[TypeOfEntities](/pages/createpage.action?spaceKey=cadnet&title=TypeOfEntities&linkCreation=true&fromPageId=20381706)' rasterization property |Enhancement |
|CADNET-137 |[Converting DWG to PDF is generating extra page at the end of PDF file](http://www.aspose.com/community/forums/thread/775407/aspose.cad-1.1.0-extra-blank-page-created-when-convering-dwg-to-pdf.aspx)|Enhancement |
|CADNET-136 |Low quality of pdf files generated by GDI Pdf exporter |Enhancement |
|CADNET-133 |Review and adapt architecture to CAD domain |Enhancement |
|CADNET-132 |Compound objects of a DGN drawing are not displayed |Enhancement |
|CADNET-130 |No GDI Pdf exporter available for DGN format |Enhancement |
|CADNET-127 |Add shortcuts to online documentation and other useful aspose resources |Enhancement |
|CADNET-126 |DGN exporter doesn't respect pen color |Enhancement |
|CADNET-125 |Text shifts unexpectedly during Model export |Enhancement |
|CADNET-122 |AutomaticLayoutsScaling does not work correctly |Enhancement |
|CADNET-120 |[Some Patterns are missing while converting DXF to PDF format](http://www.aspose.com/community/forums/thread/752283/some-hatch-patterns-displaying-incorrectly.aspx)|Enhancement |
|CADNET-117 |[GC overhead limit exceeded - exception when loading DWG file](http://www.aspose.com/community/forums/thread/747056/hang-loading-dwg-file.aspx)|Enhancement |
|CADNET-108 |Improve Image.[GetFileFormat](/pages/createpage.action?spaceKey=cadnet&title=GetFileFormat&linkCreation=true&fromPageId=20381706) method to support raster image types |Enhancement |
|CADNET-106 |Improve exception text and improve exception architecture |Enhancement |
### **Usage Examples**
**CADNET-164 Loading DGN file is throwing exception**

{{< highlight java >}}

 var file = "DgnFile_v8.dgn";

try

{

  // this will throw on drawings stored in version 8 format

  using (var image = (DgnImage)Image.Load(file))

  {

  }

}

catch (ImageLoadException e)

{

   Console.WriteLine(e.InnerException.Message == "The Dgn version isn't valid. Only Dgn: V7 are currently supported.");

}

{{< /highlight >}}

**CADNET-134 Integrate metering module to promote new sales model for Aspose.CAD**

{{< highlight java >}}

   MeteredLicenseManager.Connect("yourPublicKey","yourPrivateKey");

  ....

  // do some load save operations

  Thread.Sleep(timeout);

  MeteredLicenseManager.GetConsumptionQuantity();

{{< /highlight >}}