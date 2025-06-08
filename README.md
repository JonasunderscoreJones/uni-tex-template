# uni-tex-template

The Latex Template for my University Assignments.

## Overview
- Inclusion of all required packages and configuration
- Customized Header with all required information and fields for assignment submission
- Single-File config for simplicity

## Usage
This Template works for 1 to 4 credited Authors.

The default config is of the 2-Author variant. The additional 2 configurations are clearly commented in the Preamble of the document.

To use a 1, 3 or 4 Author configuration, do as follows:

1. Comment out the enabled config as follows:
```tex
% Default config
% \lhead{Subject Name\\Term}
% \chead{\bfseries{\vspace{0.5\baselineskip}Assignment Title}}
% \rhead{Name of 1st Author, Matr. Nr of 1st Author\\Name of 2nd Author, {Matr. Nr of 2nd Author}}
```
2. Choose Your desired configuration and uncomment it as follows:
    - Single-Author:
        ```tex
        % UNCOMMENT TO USE: Config for Single Author
        \lhead{\vspace{0.5\baselineskip}Assignment Title}
        \chead{\bfseries{Subject Name\\Term}}
        \rhead{\vspace{0.5\baselineskip}Name of 1st Author, Mtr. Nr of 1st Author}
        ```
    - 3- or 4-Authors:
        ```tex
        % UNCOMMENT TO USE: Config for 3-4 Authors
        \lhead{Name of 1st Author, Matr. Nr of 1st Author\\Name of 2nd Author, Matr. Nr of 2nd Author}
        \chead{\bfseries{\vspace{0.5\baselineskip}Subject Name\\Assignment Title}}
        \rhead{Name of 3rd Author, Matr. Nr of 3rd Author\\Name of 4th Author, Matr. Nr of 4th Author}
        ```
        *Note*: For this variant with a 3 Author config, simply remove the last part of the `\rhead` tag with the linebreak!
3. Recompile!

# License
`Creative Commons Attribution 1.0`
