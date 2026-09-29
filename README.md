# Margaret Lei's website for MDS

## What this repository is

This repo contains the files and code necessary to create my website for MDS.

## Required installations and versions
- Quarto 1.10.18
- uv 0.12.9
- R 4.6.1
- RStudio 2026.8.2.200

## How to build the site

Enter the following in terminal:

```bash
git clone https://github.com/margaretxlei/margaretxlei.github.io.git
cd margaretxlei.github.io
uv sync
```

Open R Studio and open the project in a new session. Run the following in the console:

```r
renv::restore()
```

Return to terminal and enter the following:

```bash
uv run quarto render
```

The built site lands in the `/docs/` folder of the repository.  

\
Enter the following command in terminal to open and preview the site locally:
```bash
uv run quarto preview
```

## Data sources

The blog posts use the Palmer Penguins data. The website needs Internet access to fetch the data. Citation below:

>Horst AM, Hill AP, Gorman KB (2020). palmerpenguins: Palmer Archipelago (Antarctica) >penguin data. R package version 0.1.0. https://allisonhorst.github.io/>palmerpenguins/. doi: 10.5281/zenodo.3960218.

Data accessed via the R package website linked above and the palmerpenguins Python package, available by [CC-0](https://creativecommons.org/share-your-work/public-domain/cc0/) licence.