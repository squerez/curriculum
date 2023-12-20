# scott-clark's CV template

This LaTeX template, originally created by Scott Clark, facilitates the creation of a professional resume or CV. 
The Makefile provided automates the compilation process to generate a PDF file from the LaTeX source code.
For more information, visit [Scott Clark's GitHub repository](https://github.com/sc932/resume).

## Requirements

Before using this template, ensure you have the following dependencies installed:

- **TeX Live**: A comprehensive distribution of LaTeX.
- **texlive-latex-extra**: Additional LaTeX packages.

### Installation

To install the required packages on a Debian-based system, run:

```bash
make install
```

This command will use `apt-get` to install `texlive` and `texlive-latex-extra`.

## Generating the Resume/CV

### Generating the CV 

To generate the PDF file from the LaTeX source code, use the following command:

```bash
make cv
```

This command will invoke `pdflatex` to compile the `template.tex` file and produce the `template.pdf`.
It will also open the `template.pdf` file, displaying the final resume or CV.

### Cleaning Up

By default, generating the CV will remove intermediate files generated during the compilation process, but in case you explicitly need to clean-up, run:

```bash
make clean
```

This will remove files with extensions such as `.aux`, `.log`, `.out`, and others.


## Additional Notes

- Customize the `template.tex` file to input your personal information, work experience, education, etc.
- For advanced customization, refer to LaTeX documentation or seek additional templates and resources.
