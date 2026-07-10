# LaTeX File Template

## 1 Introduction

Thank you for choosing to use LaTeX File Template. If you find any bugs or want some feature not currently included, then my contact information can be found on my GitHub: https://github.com/MatthewEmer.

This document is intended for academics (with special focus on those in the fields of computer science or mathematics) who want to write papers or other related documents in a consistent format which ties in with standard practises from other published papers. This guide consists of setup instructions to download the files and create your first document, before moving onto the custom commands/environments designed to speed up academic writing. Before using this guide, I would suggest that you have some practise with some basic LaTeX commands using a guide such as https://www.overleaf.com/learn.

This guide is accurate as of Version 3.0.0.

## 2 Document Setup

The actual LaTeX file template is contained in the folder The Template and consists of four files: *template.tex*, *_documentContent.tex*, *_appendix.tex*, and *template.pdf*. To use the template, all four files must be downloaded and placed in the same folder.

### 2.1 Project Files
#### 2.1.1 _appendix.tex

This file allows you to add an optional appendix to the end of your document which is not counted towards your page count. By default it contains a unnumbered part title which has been inserted into the table of contents.

#### 2.1.2 _documentContent.tex

This file allows you to add all the main content of the document you are trying to write. It will be inserted after the table of contents, but before the appendix (if you choose to add one). By default it contains an example section and definition. Only pages in this file are counted towards the page count of the document.

#### 2.1.3 template.pdf

This file contains the output of the LaTeX compiler. If you want to rename this document while still working on it, then delete this version, alongside any build files your compiler has created and change the name of *template.tex*. 

#### 2.1.4 template.tex

This file sets up the structure of the document, as well as acting as a compiler for the other two *.tex* files, ensuring they get inserted into the right sections of the document. When creating your document, you need to edit lines 12-15 of this file to create the title page, alongside the document header and footer, as described in the table below.

| Line | Variable Name | Description |
|---|---|---|
| 12 | thetitle | The document’s title. This will be placed in the header. |
| 13 | thesubtitle | The document’s (optional) subtitle. This will be placed in the header. |
| 14 | theauthor | The list of authors. This will be placed in the footer. |
| 15 | thedate | Replace the code if you want a static date rather than date of last compile. |

### 2.2 Optional Files

#### 2.2.1 Storing Images

If you choose to include figures in your project, then you will need to create a subfolder labelled *Images*
where you can place the image files for the project.

#### 2.2.2 GitHub Repositories

If you are placing the document within a GitHub repository, you may want to copy over the *.gitignore* from
this repository as it is set up to ignore any LaTeX build files.

## 3 Custom Commands
### 3.1 General Tools
#### 3.1.1 Element Spacing
#### 3.1.2 Text Formatting
#### 3.1.3 Date Formatting
### 3.2 Tables and Figures
#### 3.2.1 Inserting Tables
#### 3.2.2 Inserting Figures
#### 3.2.3 Referencing Tables and Figures
### 3.3 Academic Environments
#### 3.3.1 Basic Environments
#### 3.3.2 Environments with Proofs or Solutions
#### 3.3.3 Sub-Environments
#### 3.3.4 Customisable Environments
#### 3.3.5 Referencing Environments
### 3.4 Mathematics
#### 3.4.1 Basic Mathematics Notation
#### 3.4.2 Vectors and Matrices
### 3.5 Computer Science
#### 3.5.1 Set Notation
#### 3.5.2 Algorithms