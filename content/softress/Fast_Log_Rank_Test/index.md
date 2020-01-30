+++
title = "Fastlogranktest"
date = 2020-01-30
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
#tags = ["drug repurposing", "systems medicine"]

# Project summary to display on homepage.
summary = "Fastlogranktest is a project that has the goal to calculate Log-Rank-Tests in the shortest possible time. The possible application of this is very versatile and is recommended if your program or your analysis needs to use the log-rank-test very often and it takes up too much runtime. On the one hand, an efficient algorithm has been implemented in C++ code to calculate a single Log-Rank-Test as fast as possible, but also multithreading has been implemented to calculate several Log-Rank-Tests at the same time."

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
[Python package](https://pypi.org/project/fastlogranktest/) offers a fast alternative to the logrank_test()-method from the well-known liflines.statistics package, by using C++ code in the background. If you have used this method before and it makes the code very slow, all you have to do is install the package fastlogranktest and use the method of the same name with exactly the same usage. Furthermore, if you want to calculate many Log-Rank-Tests, you can use threading to parallelize them and thus calculate even faster with the multi_logrank_test()-method. 

[R package](https://cran.r-project.org/web/packages/fastlogranktest/index.html) offers the same methods as the Python package and is based on the same C++ code. So if you calculate many Log-Rank-Tests in R, you can also use the fastlogranktest package, especially if you have runtime problems and have used for example the survival package so far.

C++ Programm can be very useful if you have survival data and no classification of the groups yet. All arbitrary group classifications and the survival data can be given with the help of a simple tab-separated text-file and you will get back a text-file with the corresponding p-values in the shortest possible time. From this file you can decide which group classifications could be interesting for further analyses. Since this program is based on multithreading, it is recommended to run it on systems with as many threads as possible.
