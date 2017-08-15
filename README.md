# DevExpress End-User Documentation

In addition to [developer documentation](https://www.devexpress.com/Support/Documentation/), DevExpress also provides **end-user documentation** for its Desktop (Windows Forms & WPF) and ASP.NET products. This documentation contains information on individual user interface elements (such as grids, navigation panes, data editors, charts, etc.), and provides instructions for end-users about how to solve the most-common tasks with these interface elements.

The main goal of this repository is to provide developers who create applications with DevExpress .NET controls with drafts for their own help documents. You can distribute the included help documents to your end-users "as is" or create documentation for your own products based on them. Help documents are provided as markdown files, which are easy to edit and reuse. The [docfx.json](docfx.json) file allows you to build a documentation website using the [DocFX](https://dotnet.github.io/docfx/) documentation generation tool.

## Browse End-User Documentation
You can browse the end-user documentation repository content starting from the [index.md](index.md) document. The documentation is divided into four sections, each having an individual table of content. A sample web site which is built based on markdown files from this repository is published at [devexpress.github.io/dotnet-eud](https://devexpress.github.io/dotnet-eud/).

## Build Your Own Documentation Website
Follow the steps below to create the documentation website for your application. 
- Download and install the [latest version of DocFX](https://github.com/dotnet/docfx/releases). 
- Choose the repository branch corresponding to the DevExpress controls version your application is based on. The **master** branch corresponds to the version which is currently in development and generally there is no need to use it.
- Clone this repository to your computer, or download and extract the ZIP file.
- If you want to reuse the end-user documentation as is, skip this step. Otherwise, make the required changes that may include:
  - removing files that are not needed in your documentation;
  - adding new documents specific to your application;
  - changing screenshots to match your app UI;
  - creating a [custom DocFX template](https://dotnet.github.io/docfx/tutorial/howto_create_custom_template.html);
  - etc...
  > Do not forget to update *toc.yml* ([table-of-content](https://dotnet.github.io/docfx/tutorial/intro_toc.html)) files if you have created or removed certain topics.
- Open the console window, change the current directory to the repository root folder and call the DocFX executable with the *build* and *docfx.json* parameters. Optionally, you can also pass the *--serve* command line switch - it allows you to immediately view the generated website at http://localhost:8080 when the build process is completed. The documentation content will be placed into the *\_site* folder.
    ```
    docfx.exe build docfx.json --serve
    ```
- Finally, you can deploy the created documentation to any web server or even browse the documentation directly from the local file system, as DocFX creates static HTML files only.

## Build Printer-Friendly PDF Files
If your end-users require hard copy documents, you can create PDF files.
- Ensure that you can successfully build a website with DocFX (see the [previous section](#build-your-own-documentation-website)).
- Download and install the [wkhtmltopdf](https://github.com/wkhtmltopdf/wkhtmltopdf) tool.
- Open the console window and add the **wkhtmltopdf** executable path to the %PATH% environment variable:
    ```
    set PATH=%PATH%;C:\Program Files\wkhtmltopdf\bin
    ```
- Change the current directory to the repository root folder and call the DocFX executable with the *pdf* and *docfx.json* parameters. A separate PDF file will be generated under the *_pdf* subfolder for each table-of-content file.
    ```
    docfx.exe pdf docfx.json
    ```

## Obtain End-User Documentation for Versions Prior to 17.1
This repository provides help files for DevExpress product versions starting from 17.1. End-user documentation for previous versions is published in CHM and PDF formats at https://www.devexpress.com/Support/Documentation/download.xml?platform=user-dev-docs.

## Licensing Questions
According to the [End-User Documentation License Agreement](LICENSE.md), you have a permit to modify, re-use and distribute this end-user documentation.
