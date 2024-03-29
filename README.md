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
7)  Bulk transcriptomics fundamentals 
- https://doi.org/10.1093/bib/bbac529
- annualreviews.org/doi/abs/10.1146/annurev-biodatasci-072018-021255
9)	Tidy transcriptomics https://stemangiola.github.io/bioc2021_tidytranscriptomics/articles/tidytranscriptomics.html
10)	Single-cell analyses using Seurat 
- https://satijalab.org/seurat/articles/pbmc3k_tutorial.html
- https://satijalab.org/seurat/articles/integration_introduction.html
11)	Code debugging in R/Rstudio https://support.rstudio.com/hc/en-us/articles/205612627-Debugging-with-the-RStudio-IDE
12)	Design matrix https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7873980/
13)	Unit tests when building packages/software with `testthat` https://testthat.r-lib.org/

# Strategy to build a document

1) Create a Google doc
2) create an automatic table of content (based on headers, google how to do it)
3) Write the headers of the main sections (whatever the requirements are, e.g. introduction, rationale, methods, results)
4) Write the headers of the subsections
5) Write the headers of the sub-subsections
6) Write the titles of the paragraphs for each sub-subsection (these describe what each paragraph includes, a the end, before submission, they will be deleted)
7) Ask for feedback from the supervisor, and redo points 2-6 until there is no more feedback
8) Fill the content of the paragraphs without eliminating any headers (each paragraph should be similar in length, if not, create more (6))

## How should the Introduction section be organised

### Paragraph 1: General Introduction
Start with a broad and concise statement that introduces the general field of study and the overarching problem you are addressing. This paragraph should provide context for your research and highlight the significance of the topic.

### Paragraph 2: Specific Problem
Narrow down the focus from the general field to the specific problem or gap in knowledge that your study aims to address. Explain why this problem is important, highlighting any limitations or gaps in current methods, techniques, or approaches.

### Paragraph 3: Relevance and Impact
Emphasize the significance of solving the specific problem you've identified. Discuss the potential impact of addressing this problem on the broader scientific community, technological advancements, or real-world applications. Highlight the potential benefits and outcomes of your research.

### Paragraph 4: Previous Approaches
Briefly summarize the existing methods, techniques, or approaches that have been used to tackle the problem. Discuss their strengths and limitations, and explain why these approaches are not sufficient or why there is a need for a new method.

### Paragraph 5: Transition to Your Method
Introduce the innovative method or approach that you are presenting in your study. Highlight the key features that make your method unique, and explain how it addresses the limitations of existing approaches. You can briefly mention the advantages and potential contributions your method brings to the field.

### Paragraph 6: Objectives of the Study
Clearly state the objectives or goals of your research. What specific outcomes do you aim to achieve with your new method? This paragraph helps set expectations for the reader about what they can expect from the rest of your paper.

### Paragraph 7: Structure of the Paper
Conclude your introduction by providing a brief overview of how the paper is structured. Mention the main sections or components of your article, including the methods, results, discussion, and any other relevant sections.

Remember, the introduction should be clear, concise, and engaging. It should provide enough information for the reader to understand the context and importance of your research while also generating interest in the rest of the paper. Make sure to smoothly transition between paragraphs and maintain a logical flow of ideas. Additionally, ensure that your writing is free of jargon and is accessible to a broad audience of researchers in related fields.

# Strategy to build a presentation
1) Set up the number of slides to ~70% of the number of presentation minutes (excluding questions; e.g. 30 minutes = ~20 slides).
2) Write the content/title of each slide as bullet points.
3) The title should be active (e.g. NK cells in cancer are enriched for Interleukin-6) rather than descriptive (e.g. UMAP of NK cells in cancer versus healthy).
4) One of the first slides should show the importance and the rationale of your work (why the world needs what you are doing and why nobody else can do it).
5) Avoid acronyms and abbreviations anywhere in the presentation.
6) All plots should have X and Y-axis titles, including units (e.g. scaled gene-transcript counts, ml, mol/ml).
7) All text in the figures should be at least 9 points (figures should be exported in a way to control for that size).
8) Aim to have the talk rehearsed at least one week before. The following are useful steps to get ready:
 - Write down what you would say for each slide in a concise and elegant way
 - Practice first without time, a few times, and write down one/two words per slide that you keep forgetting and/or are good hooks for a smooth presentation (e.g. a word that has a lot of meaning, but that if you forget you will need to use 20 words to express the same meaning)
 - Practice a few times with time, and realise if you need to cut down material
 - Practice a few times recording yourself with video, and realise what you can improve for the execution
 - Aim not to have to read any notes during your presentation
10) Ask colleagues about a few questions they might have, and do a good literature review about how many laboratories have used your (or alternative) techniques/principles applied to your or other diseases.

# Coding notes
- When you meet problems, try to solve them yourself first. (google; start with a simpler example), then discuss it with the supervisor.
- Work within an R project all the time (The R project must be connected with a github repository)
-	Any big R object/variable OR an R object/variable that takes a significant amount of time to compute (e.g. takes > 15 minutes OR data before a big change of annotation) should be saved as rds with a meaningful name and date. To save do job::job({saveRDS(…)}).
-	When working on a project, especially an R package, set up `git`/`github` environment, and **never** duplicate the working directory to try out things; just use `git` to build different branches. For example, your R package is called `myR`, and although `myR` has been setup with `git`, you copy `myR` to `myR_temp` or `myR_new` so you can change a few things and see if they work. This is a bad practice and should be avoided.
-	Email the helpdesk to make sure you are working on the right hard drive that has a backup and is not your home directory, which does not have much drive space.
-	Commit with git at the end of the day (or more frequently) ONLY the R files to your github repository
-	Nowhere in the variables or file names should there be a space character “ “ 
- Variable names and file names should not include acronyms, and if your cousin opens your code should be able to understand what the variable is from the variable name
--  A bad example is df, which is not a word included in the English dictionary
--  A good example is b_cell_filtered, b_cell_pseudobulk, b_cell_for_boxplot 

# Further notes
- Scientific writing course https://www.coursera.org/learn/sciwrite
- ForZOOM, always share the screen and not the single application
- For ZOOM, always ask to start the recording at every meeting at the very beginning

# Figure, attention to detail

It is important to develop extremely good attention to detail for image composition. In terms of design, alignment, harmony, information concentration, consistency of fonts, line thickness, and line colour.

Have a look at these two images and spot all the details that make them different

1            |  2
:-------------------------:|:-------------------------:
<img width="699" alt="image" src="https://user-images.githubusercontent.com/7232890/222042169-cb1c9a22-97d0-45ee-966c-0cbab7b4bf0b.png">  |  <img width="679" alt="image" src="https://user-images.githubusercontent.com/7232890/222042234-cb93128e-0f30-48f1-a30c-771b068f7376.png">

1            |  2
:-------------------------:|:-------------------------:
<img width="441" alt="image" src="https://user-images.githubusercontent.com/7232890/222043610-d79e079b-0cd4-42f2-b17e-94e38e4beb52.png"> | <img width="403" alt="image" src="https://user-images.githubusercontent.com/7232890/222043751-0c252d58-7d84-40c2-85b3-9d7c2dcf7bdf.png">





# How to close your project

Please add the following documentation to the README

- list all directories in the local git directory (some of the will be also present in github) and what they include
- list all R scripts and declare what they do in lay terms, what inputs they take and what outputs they produce
- list all local data files and what they include
- Add all the steps with code for reproducing your results from raw data. For example,

```bash
# Preprocess the data
Rscript MY_SCRIPT.R

# Execute differential analyses for XXX dataset
makeflow XXX

...
```

- Try to reproduce your own documentation/code and see if the results/figures get produced as expected without errors (maybe do all this in a copy of your repository to avoid to overwrite your results).

