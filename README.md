# PPOL567 Project

This is a group project by Lucienne L. Julian, Peijin Li, Sonali Subbu Rathinam and Aaron Genin.

Project website: https://peijin0405.github.io/WorldNews-Subreddit-Analysis-PySpark/

## Project overview and objective

Over the rest of the semester, you will work with the [Reddit Archive data](https://files.pushshift.io/reddit/) from January 2022 through the end of January 2023, representing about 400GB of uncompressed text parquet data. For a sneak peek of the data, you can download sample files of the submissions and comments:

* [Submissions sample JSON](https://files.pushshift.io/reddit/submissions/sample.json)
* [Comments sample JSON](https://files.pushshift.io/reddit/comments/sample_data.json)

This is a very rich dataset and it is up to you to decide how you are going to use it. You will select one or more topics of interest to explore and use the Reddit data **and external data** to perform a meaningful analysis. 

You will use Spark on EMR (and SageMaker) and Python to analyze, transform, and process your data and create one or more analytical datasets. **These are the only tools permitted.**

In your work as data scientists, in addition to doing modeling and machine learning work, you will be responsible (either individually or as part of a team) for providing the following as part of a project:

* **Findings:** what does the data say?
* **Conclusions:** what is your interpretation of the data?
* **Recommendations:** what can be done to address the question/problem at hand

Your analysis will focus on the first two above. It should allow the audience to be able to understand the topic you are analyzing, presenting and discussing. The objective is to find a topic of interest, work with the data, and present it to an audience that may not know very much about the subject using a data-driven approach.

## Milestones

The project will be executed over several milestones, and each one has a specific set of requirements and instructions located in the `instructions/` directory.

There are four major milestones (click on each one for the approprate instructions and description):

1. [Milestone 1: Define the questions and Exploratory Data Analysis](instructions/eda.md)
1. [Milestone 2: NLP and external data overlay](instructions/nlp.md)
1. [Milestone 3: Machine Learning](instructions/ml.md)
1. [Milestone 4: Final delivery](instructions/final.md)

All of your work (with the exception of the first milestone) will be done within this team GitHub repository, and each milestone will be tagged with a specific [release tag](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository) by the due date.  

## Repository structure

You will work within an **organized** repository and apply coding and development best practices. The repository has the following structure:

```.
├── LICENSE
├── README.md
├── code/
├── data/
├── img/
├── instructions/
└── website-source/
└── docs/
```

### Description

* The `code/` directory is where you will write all of your scripts. You will have a combination of PySpark and Python notebooks, and one sub-directory per major task area. You may add additional sub-directories as needed to modularize your development.
* The `data/` directory contains.
* The `img/` directory contains screenshots for the instructions. **You will not edit this directory.** 
* The `instructions/` directory contains all project instructions. The best way to see the instructions is to start from the [milestones](#milestones). **You will not edit this directory.** 
* The `docs/` directory where the final website will be built. Any website asset (image, html, etc.) must be added to this directory.
    - **You do not need to serve the website, although you can do so if you wish. However, this naming convention may not work.**
    - The `docs/` directory will automatically be picked up by GitHub Pages so your website will be rendered automatically. If you do not wish to render your website, talk to your instructor to disable publishing GitHub Pages for your repo.
    - If you would like to publish your website to another hosting service such as gu-domains then you can simply copy (scp) the `docs` folder to your website.
* The `website-source/` is where you will develop the website using your preferred method. It must render in `docs/`.

## Set-up the Spark on SageMaker Studio Notebook

Follow instructions in [this lab](https://classroom.github.com/a/L_WtbRi3) to do this. Experiment with a subset of your data in a SageMaker Studio notebook and when your code is working you can switchover to the EMR cluster for working with the entire dataset of interest.

## Set-up the Spark on EMR

Follow instructions in [this lab](https://aa1603.georgetown.domains/ppol567/labs/04-labs.html) to do setup an EMR cluster. Remember that setting up an EMR cluster and working with it is costly (in terms of time and money) so first experiment on SageMaker Studio and only then move to EMR cluster.

## Code

* Your code files must be well organized
* Do not work in a messy repository and then try to clean it up
* In notebooks, use Markdown cells to explain what you are doing and the decisions you are making
* Do not write monolithic Notebooks or scripts
* Modularize your code (a script should do a single task)
* Use code comments
* Use functions to promote code reuse


## Delivery mechanism

The output of the project will be delivered through a self-contained website in the `website/` subdirectory, having `index.html` as the starting point. You will build the website incrementally over the milestones.

[Read the website requirements.](instructions/website.md)

## Evaluation

The project will be evaluated using the following high-level criteria:

* Level of analytical rigor at the graduate student level
* Level of technical approach
* Quality and clarity of your writing and overall presentation


### Grading rubric

- If a deliverable exceeds the requirements and expectations, that is considered A level work.
- If a deliverable just meets the requirements and expectations, that is considered A-/B+ level work.
- If a deliverable does not meet the requirements, that is considered B or lesser level work.

Deductions will be made for any of the following reasons:

- There is lack of analytical rigor:
    - Analytical decisions are not justified
    - Analysis is too simplistic
- Big data files included in the repository
- Instruction are not followed
- There are missing sections of the deliverable
- The overall presentation and/or writing is sloppy
- There are no comments in your code
- There are absolute filename links in your code
- The repository structure is sloppy
- Files are named incorrectly (wrong extensions, wrong case, etc.)

## Samples projects from previous years

* https://mitalishah.georgetown.domains/BigData.html

* https://hss0727.github.io/502-project-group23/index.html#projectIntroduction

* https://gu-anly502.github.io/fall-2022-reddit-big-data-project-project-group-27/

* https://hjia.georgetown.domains/502_project/index.html

