# Moved to https://codeberg.org/rahguzar/latex-refs
# latex-refs: Insert references in LaTeX documents using labels in the pdf

While writing a latex document, the easiest way to find an equation, figure or section I want to reference is to look at the generated pdf. But that doesn't tell me the label LaTeX needs. This package provides the ability to match the labels in the TeX file with those in the pdf,so that one can use the label in pdf to insert the one in TeX file. This is done with the help of aux file and this package provides function to parse it. The code (at least for now) assumes that the hyperref package is in use.

In addition it provides a simple `completing-read` based interface for entering references which can be entered using the label as it appears in the pdf (or more accurately the aux file.)

**TO DO**: Improve the context provided to the labels.

**TO DO**: Implement a synctex based preview for the labels. This might not be possible to do well since synctex does seem to always generate correct locations and it might have unacceptably high latency. It will be really nice to have so worth investigating.
