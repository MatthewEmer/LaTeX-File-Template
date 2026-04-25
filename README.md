# LaTeX File Template

This LaTeX file template is a clean, easy to use template, with multiple custom commands and formatting that makes creating LaTeX documents quicker and easier than other templates. Specifically, this is the template I have designed for creating lecture notes and assignment submissions for my work as a BSc Computer Science student at Durham University. As a result, there are plenty of functions/packages aimed at making STEM-centered documents.

## Features

- **Title Page Customisation**: Easily set the title and author(s) for the document, set the publication date automatically, and add an optional subtitle.
- **Custom Headers & Footers**: Headers containing the paper's title and subtitle, footers containing the author(s) names' and the page number for easy document navigation.
- **Content Separators**: Custom tool for separating content on the page.
- **Coloured Text**: Improved text colour tools automatically return to black after the coloured text.
- **Formatted Number Sets**: Simplified commands for adding number sets into your equations.
- **Custom Academic Formats**: Custom formats for common academic environments such as definitions, theorems, or lemmas. 
- **Simplified Commands**: Custom commands set up to make inserting images and pseudocode easier, being able to insert them in one line.

## Documentation

### Setup

1. Go to Releases and download the latest release from the repository.
2. Open *blanktemplate.tex* and find lines 146-149. 
3. Edit the values in the second set of curly brackets on each line to edit the title page, headers, and footers.
4. Find line 170 and start adding the main content for the document.

### Custom Functions

#### \colour
Changes the text colour of the given text to a specified colour before returning to black.

*Parameters*
- #1: Text Colour - the colour to change the text to (See LaTeX's website for colour options).
- #2: Text - the text to be coloured.

#### \separate
Adds a horizontal gap between two bits of content, then removes the indent on the new content (especially useful for separating text).

*Parameters*
- #1: Distance - the distance in points to separate the content by.

#### \R, \N, \C, \Q, \Z, and \I
Outputs the corresponding number set symbol.

*Parameters*
- n/a

#### \definition, \example, \conjecture, and \proof
Sets out a definition, example, conjecture, or proof environment for an academic paper.

*Parameters*
- #1: Number - the number of the definition, example, conjecture, or proof.
- #2: Content - the content for the definition, example, conjecture, or proof.

#### \numberedentry
Sets out a custom entry environment for an academic paper.

*Parameters*
- #1: Number - the number of the entry.
- #2: Entry Type - the type of the numbered entry.
- #3: Content - the content for the entry.

#### \theorem and \lemma
Sets out a theorem or lemma environment for an academic paper with corresponding proof.

*Parameters*
- #1: Number - the number of the theorem or lemma.
- #2: Theorem/Lemma - the actual theorem or lemma.
- #3: Proof - the proof for the theorem or lemma.

#### \insertimage
Places an image on the page.

*Parameters*
- #1: Image - the file path for the image.
- #2: Caption - the image caption.
- #3: Width - the width of the image, relative to the page width.

#### \insertalgorithm
Places a pseudocode algorithm on the page.

*Parameters*
- #1: Name - the name of the algorithm.
- #2: Input - the input for the algorithm.
- #3: Output - the output of the algorithm.
- #4: Code - the code for the algorithm.

#### \inserttable
Places a table on the page.

*Parameters*
- #1: Formatting - how many columns, and their borders.
- #2: Caption - the caption for the table.
- #3: Headers - the labels for each column.
- #4: Content - the main content of the table.
