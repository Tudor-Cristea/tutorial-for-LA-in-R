# Tutorial for Learning Analytics in R

Chapter 3 of my PhD dissertation (Eindhoven University of Technology, 2025), written for researchers with little or no programming experience.

## Main objective

When I started my PhD, I had no experience in programming or working with educational data. I learned these skills during my PhD, and this tutorial aims to help others in a similar position. It is written for researchers in educational fields, particularly in Learning Analytics (LA), who have little or no experience with student trace data.

Beginners can often explain a subject better than experts. They offer fresh perspectives, use relatable language and give simplified explanations that resonate with other novices. They also remember the challenges they faced while learning, which helps them anticipate common obstacles, and they are less likely to overlook basic concepts that experts take for granted.

In this tutorial, I present all the steps I followed in small, digestible chunks, with example datasets and code snippets. I use synthetic example data that mirrors what a Learning Management System (LMS), in this case Canvas, records about students, and I use R for the analysis. The concepts and explanations also apply to other LMSs and programming languages. Programming is not the main focus of this tutorial, but you will need some:

- **Part 1** covers the basics of R and of programming in general. Experienced programmers can skip it, which is why it is not included in my dissertation.
- **Part 2** covers cleaning and pre-processing the trace data to make it ready for analysis, and is included in my dissertation.

This tutorial reflects my own journey, from the first time I opened an educational dataset to the publication of scientific papers based on it. If you are looking for specific analyses and expert explanations, I highly recommend *Learning Analytics Methods and Tutorials: A Practical Guide Using R* (Saqr & López-Pernas, 2024), which I consider the best guide to Learning Analytics in R available today: <https://lamethods.github.io/>

## Related chapters

This tutorial also introduces the methods used in the next two chapters of my dissertation. Each of those chapters has its own methods section; this tutorial shows, in more detail, the steps I took before reaching that point.

- **Chapter 4:** *Unobtrusive measurement of self-regulated learning: A clickstream-based multi-dimensional scale* (Education and Information Technologies, 2024). Code: <https://github.com/Tudor-Cristea/Unobtrusive-COPES-paper>. Paper: <https://doi.org/10.1007/s10639-023-12372-6>
- **Chapter 5:** *Dynamics of self-regulated learning: The effectiveness of students' strategies across course periods* (Computers & Education, 2025). Code: <https://github.com/Tudor-Cristea/pattern-paper-scripts>. Paper: <https://doi.org/10.1016/j.compedu.2025.105233>

## What's in this repository

| File | Content |
|---|---|
| `Chapter 3, Part 1, The Basics` (.Rmd, .html, .docx) | Part 1: the basics of programming in R |
| `Chapter 3, Part 2, Advanced` (.Rmd, .html, .docx) | Part 2: trace data pre-processing |
| `example_*.xlsx`, `example_parquet.snappy.parquet` | Synthetic example data used in the tutorial |
| `req_crs_disc_assgn_quiz.csv` | The merged dataset that Part 2 produces, so you can check your result |

## How to use it

Read the tutorial in the .html files (download them and open them in your browser) or in the Word versions. To run the code yourself, download the repository (Code → Download ZIP), open the .Rmd files in RStudio and point the file paths in the code to the folder where you saved the files. You need these R packages:

```r
install.packages(c("tidyverse", "readxl", "arrow"))
```

## Example data

The example files are synthetic: I created them for this tutorial. They mirror the structure of a Canvas data export (35 page views from 4 fictional students, plus related course, assignment, quiz, file and discussion records) but describe no real students, courses or posts. Because no real people are involved, the data can be shared and reused freely.

## Licence

Code: MIT (see LICENSE). Tutorial text and example data: CC BY 4.0, so anyone may reuse them with credit.

## How to cite

Cristea, T. (2026). *Tutorial for Learning Analytics in R* (Version 1.0.0). Zenodo. https://doi.org/[your DOI]
