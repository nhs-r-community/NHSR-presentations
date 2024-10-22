
# NHSRpresentations

<!-- badges: start -->
<!-- badges: end -->

This is a repository for presentations given on behalf of NHSR Community.

Individual folders will contain the presentation slides, material and a README
to explain the presentation.

Formats for the folder names will be `yyymmdd-name-of-presentation`

## Code that is applied to all slides

The code `embed-resources: true` will be applied automatically to slides so that
the html generated does not require a separate folder to be formatted. 
This code is applied to the entire repository and subfolders as it included in 
the `_quarto.yml`. 
_Note that the line `embed-resources: true` is needed in the YAML where webr is 
used as the supporting folder is generated when the Quarto code `quarto render`
is used on the Terminal_

The style for the slides is generated from the following code which is also 
run centrally from the `_quarto.yml` file:

```
title-slide-attributes: 
  data-background-color: "#43464B"
format:
  revealjs:
    theme: [default, nhsr-quarto.scss]
    logo: https://raw.githubusercontent.com/nhs-r-community/assets/main/logo/nhsr-logo.svg
    code-link: true
    css: nhsr-quarto.scss
    preview-links: true
```

Note that although this code can be used on files in subfolders, each folder
requires the `nhsr-quarto.scss` to be copied to each folder.