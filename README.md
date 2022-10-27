# Resources for students in order of priority

1)	Rstudio https://ourcodingclub.github.io/tutorials/intro-to-r/
2)	Tidyverse
  - https://www.r-bloggers.com/2021/04/tidyverse-in-r-complete-tutorial/
  - https://www.datacamp.com/community/tutorials/tidyverse-tutorial-r
  - https://campus.datacamp.com/courses/introduction-to-the-tidyverse/data-wrangling-1?ex=4
  - https://campus.datacamp.com/courses/working-with-data-in-the-tidyverse/explore-your-data?ex=1
  - https://monashbioinformaticsplatform.github.io/r-more/topics/tidyverse.html
  - https://app.datacamp.com/learn/courses/categorical-data-in-the-tidyverse
  - https://app.datacamp.com/learn/courses/machine-learning-in-the-tidyverse
  - https://campus.datacamp.com/courses/joining-data-with-dplyr/joining-tables-1?ex=1
  - https://datacarpentry.org/R-ecology-lesson/03-dplyr.html
  - https://www.analyticsvidhya.com/blog/2019/05/beginner-guide-tidyverse-most-powerful-collection-r-packages-data-science/
3)	Git tuorial https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
4)	Github tutorial https://guides.github.com/activities/hello-world/
5)	Git in Rstudio https://www.geo.uzh.ch/microsite/reproducible_research/post/rr-rstudio-git/
6)	Git/github in Rstudio (video) https://www.youtube.com/watch?v=megZYkCLMA4 
7)	Tidy transcriptomics https://stemangiola.github.io/bioc2021_tidytranscriptomics/articles/tidytranscriptomics.html
8)	Single cell analyses using Seurat 
- https://satijalab.org/seurat/articles/pbmc3k_tutorial.html
- https://satijalab.org/seurat/articles/integration_introduction.html
9)	Code debugging in R/Rstudio https://support.rstudio.com/hc/en-us/articles/205612627-Debugging-with-the-RStudio-IDE
10)	Design matrix https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7873980/
11)	Unit-tests when building packages/sorftware with `testthat` https://testthat.r-lib.org/

# Strategy to build a document

1) Create Google doc
2) create an automatic table of content (based on headers, google how to do it)
3) Write the headers of the main sections (whatever the requirements are, e.g. introduction, rationale, methods, results)
4) Write the headers of the subsections
5) Write the headers of the sub-subsections
6) Write the titles of the paragraphs for each sub-subsection (these describe what each paragraph includes, a the end before submission they will be deleted)
7) Ask feedback to the supervisor, and redo points 2-6 until there is no more feedback
8) Fill the content of the paragraphs, without eliminating any headers (each paragraph should be similar length, if not create more (6))

# Further notes
1) Variable names and file names should not include acronyms and if your cousin opens your code should be able to understand what the variable is from the variable name
2) A bad example is df, which is not a word included in the English disctionary
3) A good example is b_cell_filtered, b_cell_pseudobulk, b_cell_for_boxplot 
4) ForZOOM, always share the screen and NOT the single application
5) For ZOOM always ask to start the recording at enery meeting, at the very beginning

# How to close your project

Please add the following documentation to the README

- list all directories in the local git directory (some of the will be also present in github) and what they include
- list all R script and declare what they do in lay terms, what inputs they take and what outputs they produce
- list all local data files and what they include
- Add all the steps with code for reproducing your results from raw data. For example,

```bash
# Preprocess the data
Rscript MY_SCRIPT.R

# Execute differential analyses for XXX dataset
makeflow XXX

...
```

- Try to reproduce your own documentation/code and see fi the results/figures get produced as expected without errors (maybe do al this in a copy of your repository to avoid to overwrite your results).
