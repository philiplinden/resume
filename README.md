# Philip J. Linden
I am an engineer who is passionate about the design, analysis, and operation of
space systems and imaging technologies.

* [LinkedIn](https://www.linkedin.com/in/philiplinden/)
* [GitHub](https://github.com/philiplinden/)
* [Resume](https://github.com/philiplinden/resume/blob/master/resume.pdf)

## This Repository
This repository is the source code used to generate my resume. 

I have omitted my home address, phone number, and email address from the public
version of this document in the interest of privacy.

The TeX class and document layout may be used as a template under the 
[LPPL](https://tldrlegal.com/license/latex-project-public-license-v1.3c-(lppl-1.3c))
license. Forks of this repository are welcome.

## Compiling from TeX
To compile this document from source:

1. Ensure the following LaTeX packages are installed.
   1. titlesec (customize header styles)
   2. geometry (page layout)
   3. hyperref (insert hyperlinks)
   4. fancyhdr (fancy header and footer)
   5. lastpage (reference number of pages in doc)
   6. enumitem (fancy lists)
   7. url (insert links)
   8. fontenc (T1 font encoding)
   9. lmodern (use Latin Modern Sans Serif)
   10. fontawesome (high quality web icons)
2.  Clone this repository `git clone git@github.com:philiplinden/resume.git`
3.  Compile `resume.tex`
    1.  In [tectonic](https://tectonic-typesetting.github.io/en-US/): `tectonic -X compile resume.tex`

To use Tectonic with VS Code and LaTeX Workshop, add the following to your 
`settings.json`.
```json
"latex-workshop.latex.recipes": [
   {
      "name": "tectonic",
      "tools": [
            "tectonic"
      ]
   }
],
"latex-workshop.latex.tools": [
   {
      "name": "tectonic",
      "command": "tectonic",
      "args": [ 
            "-X", // use the V2 CLI
            "compile", // just compile the tex, don't use Tectonic.toml
            "%DOC%.tex" 
      ],
      "env": {}
      }
]
```
The `tectonic` recipe will now be available in LaTeX Workshop
for compiling `.tex` files. See the [Tectonic V2 CLI docs](https://tectonic-typesetting.github.io/book/latest/v2cli/compile.html)
for more information.
