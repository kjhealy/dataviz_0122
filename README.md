## A Three Day Remote Seminar via [Code Horizons](https://codehorizons.com/Seminars/data-visualization/).

## Information for Participants

This page contains information for seminar participants. Please read it
and follow the instructions below to install the necessary software and
course materials.

## Sign-up and Registration

-   Learn more about logistical and registration information at the
    [seminar’s home page at Code
    Horizons](https://codehorizons.com/Seminars/data-visualization/)

## Course Overview

This course will teach you how to think about good data visualization,
and how to do it. We begin with some core principles about how we see
graphs, what makes some of them better than others, and how to begin
cultivating good judgment about visualization. Then, through a series of
worked examples, you will learn how to use ggplot to make graphs piece
by piece. The emphasis throughout is on acquiring a practical feel for
and good judgement about the way ggplot can be used, from the simplest
cases to sophisticated, highly customized data visualizations.

## Learning objectives

The effective use of graphs and charts is an important way to explore
data for yourself and to communicate your ideas and results to others.
Being able to produce effective plots from data is also the best way to
develop an eye for reading and critically understanding visualizations
made by others, whether presented in academia, business, policy, or the
media. Learning how to visualize data effectively is more than just
knowing how to write code that produces figures from data. This course
will teach you how to do that. But it will also teach you how to think
about the information you want to show, and how best to present it to
your audience—including when the audience is yourself.

## Is this course for me?

You should take this workshop if:

1.  You want to understand the basic principles behind effective data
    visualizations, and how they are implemented in R and ggplot.
2.  You want to better develop your practical sense for why some graphs
    and figures work well while others do not.
3.  You want to feel more confident and fluent in ggplot, in order to
    make, refine, and effectively present good data visualizations.

## Preparation

We will be working with the most recent stable versions of R and
RStudio, as well as with a number of additional packages. You will need
to install R, RStudio, and the necessary packages on your own computer.

### Installing R and RStudio on your Laptop

-   Begin by installing R (<http://cloud.r-project.org>). Choose the
    version appropriate for your computing platform:
    -   [macOS with an Intel
        processor](https://cloud.r-project.org/bin/macosx/base/R-4.1.2.pkg)
    -   [macOS with an Apple Silicon (M1)
        processor](https://cloud.r-project.org/bin/macosx/big-sur-arm64/base/R-4.1.2-arm64.pkg)
    -   [Windows](https://cloud.r-project.org/bin/windows/base/R-4.1.2-win.exe),
    -   [Linux](https://cloud.r-project.org/bin/linux/).
-   Next, install RStudio (<http://rstudio.com>). Follow the links to
    download the [free RStudio Desktop
    edition](https://rstudio.com/products/rstudio/download/#download)
    recommended for your system.

### Installing the required additional Packages

-   Once the applications are installed, launch RStudio. Either
    carefully type in or copy-and-paste the following lines of code at
    R’s command prompt, located in the RStudio window named “Console”,
    and then hit return. In the code below, the &lt;- arrow is made up
    of two keystrokes, first &lt; and then the short dash or minus
    symbol, -.

<!-- -->

    ## Code to run at the RStudio console begins here

    my_packages <- c("tidyverse", "broom", "coefplot", "cowplot", 
                      "drat", "gapminder", "GGally", "ggforce", 
                      "ggrepel", "ggraph", "ggridges", "graphlayouts", 
                      "here", "margins", "maps", "mapproj", 
                      "mapdata", "MASS", "naniar", "palmerpenguins", 
                      "patchwork", "prismatic", "quantreg", "remotes", 
                      "scales", "sf", "socviz", "survey", "srvyr", 
                      "tidygraph", "viridis", "viridisLite")

    install.packages(my_packages, repos = "http://cran.rstudio.com")

    data_packages <- c("covdata", "congress", "kjhnet", "nycdogs")

    drat::addRepo("kjhealy")
    install.packages(data_packages, repos = "https://kjhealy.github.io/drat/")

    ## Code to run ends here

If you do not have one already, it will be useful to create a GitHub
account and obtain a GitHub Personal Access Token. (This is not required
for the course, it will just be helpful to have one.) To get set up,
read and *carefully follow* the instructions in Parts I and II of [Happy
Git With R](https://happygitwithr.com), and then also the instructions
in [Appendix B](https://happygitwithr.com/github-pat.html) of the same
document.

# The Course Packet

This repo is also the course packet. It contains the course material,
data, slides, and code for the graphs we will draw. It’s an RStudio
project. Clone it with Git or [download it as a zip
file](https://github.com/kjhealy/dataviz_0122/archive/refs/heads/main.zip)
and decompress it. To launch the project, double-click on
`dataviz.Rproj` and RStudio will open with this project ready to go.

## What’s here

### RMarkdown files

-   `course_notes.Rmd` is an RMarkdown document to get you started on
    taking your own notes for the course, and writing your own code.
-   `scratch.Rmd`is where I’ll work on examples or queries that come up
    in class.
-   The other `.Rmd` files contain all of the code snippets from the
    slides.

### The `data/` folder

Datasets we may use during the course.

### The `slides/` folder

PDF versions of the slides from the course.

# Instructor

[Kieran Healy](https://kieranhealy.org) is Professor of Sociology at
Duke University. He is the author of [Data Visualization: A Practical
Introduction](http://socviz.co) (Princeton University Press, 2019). Much
of his research has been about the social organization of exchange in
human blood and organs, cultural goods, software, and ideas. His current
work focuses on the moral order of market society, the effect of models
and measurement on social classification, and the link between those two
topics, especially in the consumer credit market. You can learn more at
<https://kieranhealy.org>
