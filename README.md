# jhsphbeamer
A beamer theme for the JHSPH Department of Biostatistics

This template is a modified version of The University of Tennessee, Knoxville theme made by Enda Hargaden and is meant to approximate the official JHSPH Power Point template, which you can view [here](https://my.jhsph.edu/Offices/ExternalAffairs/OfficeCommunications/Documents/Forms/AllItems.aspx?RootFolder=%2fOffices%2fExternalAffairs%2fOfficeCommunications%2fDocuments%2fPowerpoint%20Templates&FolderCTID=&View=%7b87F1BD1E%2d84FA%2d40B7%2d9F41%2dFD46C31048D5%7d) with a JHSPH login. 

To use this template, I would follow the directions [here](http://tex.stackexchange.com/questions/1137/where-do-i-place-my-own-sty-or-cls-files-to-make-them-available-to-all-my-te). In short, for Mac users, find where your TeX directory is using this command

`kpsewhich -var-value=TEXMFHOME`

for me this is

`/Users/jfiksel/Library/texmf`

If you don't have a `texmf` directory under Library, type

`mkdir texmf`

Eventually the path we will be working in is 

`/Users/<user name>/Library/texmf/tex/latex/local`

If you don't have any directories under texmf, do the following

```
cd texmf
mkdir tex
cd tex
mkdir latex
cd latex
mkdir local
cd local
```

You then want to have the `beamerthemejhsph.sty`, `jhsph_logo.png`, and `jhsph_shield.jpg` files inside of the local directory. You should hopefully then be able to start any beamer presentation with
```
\documentclass{beamer}
\usetheme{jhsph}

\author{My Name}

\begin{document}

<slides>

\end{document}
```

as in the example texfile. Please feel free to make any changes or submit questions!

