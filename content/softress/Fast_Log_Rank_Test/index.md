+++
title = "Fastlogranktest"
date = 2020-01-30
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
#tags = ["drug repurposing", "systems medicine"]

# Project summary to display on homepage.
summary = "Fastlogranktest is a software package providing wicked-fast implementations of the logrank test in C++, R, and Python."

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Does the project detail page use source code highlighting?
highlight = false

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "sponge_overview.png"`.
[header]
image = ""
caption = ""

+++
The [Python package](https://pypi.org/project/fastlogranktest/) and [R package](https://cran.r-project.org/web/packages/fastlogranktest/index.html) provide wrappers around the C++ implementation. Both offer a fast alternative to the standard logrank-test implementations in the liflines.statistics and survival pacakges, respectively. All you have to do is install the package fastlogranktest and use the method of the same name with exactly the same usage. Furthermore, the Python package and R package provide threading to parallelize the logrank-tests and calculate them even faster with the multi_logrank_test()-method.

The C++ programm itself allows to specify arbitrary group classifications and survival data in a simple tab-separated text-file to run many tests with a single command. The result is provided as another text file with the p-values corresponding to the specified classifications.
