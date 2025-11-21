<div align="center">

# SlicerMeta

<h3>C# API for extracting metadata from G-Code/3MF Files, designed for use with FlashForge (3D printer) software development</h3>

![NuGet Version](https://img.shields.io/nuget/v/SlicerMeta?style=flat-square&logo=nuget&label=NuGet)
![License](https://img.shields.io/github/license/Parallel-7/SlicerMeta?style=flat-square)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)

</div>

---

<div align="center">

### Maintenance Mode Notice

<p align="center">
This library is no longer under active development. Only critical bug fixes and essential functionality backports will be provided.
</p>

<p align="center">
<strong>For new projects, please use the modern cross-platform rewrite:</strong><br>
<a href="https://github.com/Parallel-7/slicer-meta">slicer-meta</a> - TypeScript + Node.js implementation<br>
Easy to work with and use on any operating system
</p>

</div>

---

<div align="center">

## Features

<table>
<tr>
<th>Feature</th>
<th>Description</th>
</tr>
<tr>
<td><strong>Slicer Metadata Extraction</strong></td>
<td>Retrieve slicer metadata including name, version, date & time, printer name, and more from all gcode files</td>
</tr>
<tr>
<td><strong>Filament Information</strong></td>
<td>Extract filament info (material type) from all gcode & 3mf files. Additional data available (color, used grams, used meters) depending on slicing software</td>
</tr>
<tr>
<td><strong>Embedded Thumbnails</strong></td>
<td>Retrieve embedded thumbnails from supported file types (3mf) and supported slicers (gcode)</td>
</tr>
</table>

</div>

---

<div align="center">

## Supported Slicers

<table>
<tr>
<th>Slicer</th>
<th>Support Status</th>
</tr>
<tr>
<td><strong>Orca-FlashForge</strong></td>
<td>Fully Supported</td>
</tr>
<tr>
<td><strong>OrcaSlicer</strong></td>
<td>Supported (not fully tested)</td>
</tr>
<tr>
<td><strong>FlashPrint</strong></td>
<td>Fully Supported (FlashForge's legacy slicer)</td>
</tr>
</table>

</div>

---

<div align="center">

## Example Usage

<table>
<tr>
<th>Step</th>
<th>Code</th>
<th>Description</th>
</tr>
<tr>
<td>1</td>
<td>var parser = new GCodeParser();</td>
<td>Create a new parser instance</td>
</tr>
<tr>
<td>2</td>
<td>parser.Parse(filePath);</td>
<td>Parse the gcode file at the specified path</td>
</tr>
<tr>
<td>3</td>
<td>parser.SlicerInfo.SlicerName</td>
<td>Access the slicer name from metadata</td>
</tr>
<tr>
<td>4</td>
<td>parser.FileInfo.FilamentType</td>
<td>Access the filament type information</td>
</tr>
</table>

</div>

---

<div align="center">

<p>Made for the FlashForge community</p>

</div>
