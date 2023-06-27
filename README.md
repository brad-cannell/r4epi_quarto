# R4Epi Quarto

A repository for the Quarto version of R4Epi.

## Useful websites:

-   [Quarto book documentation](https://quarto.org/docs/books/)
-   [My test Quarto book repository](https://github.com/brad-cannell/test_quarto_book)
-   [My test Quarto book](https://brad-cannell.github.io/test_quarto_book/)

## Rendering

We can render the files by clicking the Render button in RStudio. To render the HTML and PDF files at the same time, type `quarto render` into the terminal. 

````
```{bash}
quarto render
```
````

You can also render Quarto files with a native R code chunk.

- The input argument: The input file or project directory to be rendered (defaults to rendering the project in the current working directory).

- The output_format argument: Target output format (defaults to "html"). The option "all" will render all formats defined within the file or project.

````
```{r}
#| Render with R
#| eval: false
quarto::quarto_render(output_format = "all")
```
````

## Publishing to GitHub pages

[This article is great](https://quarto.org/docs/publishing/github-pages.html). After committing, and making sure you are on the main branch, type `quarto publish gh-pages` in the terminal.

````
```{bash}
quarto publish gh-pages
```
````
