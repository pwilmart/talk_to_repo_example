# talk_to_repo_example

Example of turning a Powerpoint talk into a repo README.md. Created by Phil Wilmarth, November 9, 2019.

---

**Pattern:**
- [optional] slide title or number
- hyperlink to slide image
- text from note for slide
- separator

---

![slide 1](images_talk/Slide1.png)

I would like to thank the organizers.

---

![slide 2](images_talk/Slide2.png)

Like many of you, I am not too excited to be on this side of the podium. Let's hope the talk goes like planned...

---

![slide 3](images_talk/Slide3.png)

I spent much of the winter creating notebooks to explain TMT data normalization and statistical testing. They are available on Github (www.github.com/pwilmart). Around the time the call for abstracts for this meeting went out, there was this Atlantic article claiming that notebooks could replace papers. That made me think that a little introduction to notebooks would be fun.

---

![slide 4](images_talk/Slide4.png)

The Atlantic article claims that notebooks can replace traditional scientific papers. What kind of notebooks are they talking about? They are not electronic lab notebooks, nor are they similar to Evernote notebooks. The notebooks are like Mathematica notebooks and their newer open source variant Jupyter notebooks. These notebooks are web server applications with some connection to a local programming environment. You create and interact with notebooks through web browsers. Notebooks can render rich text formatting, execute code blocks (typically Python or R), and display the output (graphics and text) from the code blocks. I will show you Jupyter notebooks today, but R Markdown in RStudio is conceptually very similar.

---

![slide 5](images_talk/Slide5.png)

Before you can launch notebooks, you have to install the webserver application stuff. If you install a scientific Python distribution like Anaconda, you get Jupyter notebooks to go with numpy, matplotlib, pandas, scipy, scikit learn, etc. Scientific Python distributions have many packages that are not part of the standard Python library. Anaconda makes it easier to install all of these and keep them updated. Anaconda and all of the major packages including Jupyter notebooks (www.jupyter.org) have extensive online documentation. Python support is included by default; however, support for R takes some extra installation steps.

---

![slide 6](images_talk/Slide6.png)

---

![slide 7](images_talk/Slide7.png)

But wait. R has many more ways to visualize data. We have three replicates at each time point. We can pick each time point and see how similar the biological replicates are to each other. We can use a function from the "psych" package to do multi-panel scatter plots. With a single line of code, we can get the 9-panel plots. We can compare without IRS (left) to with IRS (right).

The lower diagonal is each replicate scatter plotted against the other replicates. The red line is a linear fit. The upper diagonals are the correlation coefficients. The diagonal shows the histogram of the log2 intensity distribution, a kernel density smoother, and a rug plot. The data on the right are obviously much better than the data on the left. If the normalization works correctly, each biological replicate should be similar to the others, independent of which TMT experiment it comes from.

---

![slide 8](images_talk/Slide8.png)

The Atlantic article predicts the demise of the scientific paper, and its replacement by notebooks. I do not think we are quite there yet (if that is even possible). However, notebooks would make great supplemental files for critical parts of the data analyses that are often rather poorly described in current papers. The biological samples and processing are usually done well. Since the MCP 2004 guidelines for publishing proteomics data, mass spectrometer and chromatography steps are typically detailed adequately. Most papers also describe search program settings and protein databases accurately. The normalization of quantitative data and statistical testing steps are probably the most poorly described parts of data analyses. This is an area that can be ideally addressed by notebooks.

Notebooks can be developed as templates for quality control, normalizations, and statistical testing, and easily modified for new experiments. This would enable more rapid assessment that the sample processing and mass spectrometry worked correctly. The visualizations available for evaluating the sanity of differential expression candidates is important to do before time and money is spent on validation efforts. Or before trying to convince reviewers that your data analysis was performed correctly.

---

![slide 9](images_talk/Slide9.png)

Notebooks are really powerful; however, power does not come cheaply. There can be a tremendous amount of learning involved and that can take a lot of time. This is time that will not directly further your career, so you have to be very careful about the time spent. All of these topics have multiple books written about them, and very extensive online documentation. I find Python to be a more intuitive computer language to learn, but Python 3 is more complicated that Python 2 was. The scientific extensions are extensive. R is not much like other computer languages and learning how to be effective at coding in R can be a **lengthy** journey.

I did not have any time to talk about version control, another key component in reproducible research, but Git and Github are also big topics with lots to learn. All of these topics are pretty central to "data science", an emerging field, and this is where I have learned about them. The folks listed here are some of the key people to pay attention to in data science. Hadley is one of the most influential R programmers (ggplot2 and the tidyverse), Wes wrote the pandas table manager package for Python, and Jake has written the Altair visualization package for Python (and is local).

---

![slide 10](images_talk/Slide10.png)

Thank you for your time and attention. Please visit the Github site for complete notebook examples and more.

---

Full talk is in [this repository](https://github.com/pwilmart/Cascadia_2018)
