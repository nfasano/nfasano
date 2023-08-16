<h3 align="center">
    Nicholas Fasano
</h3>
<h3 align="center">
    nmfasano5@gmail.com | <a href="https://www.linkedin.com/in/nmfasano/" target="_blank">LinkedIn</a> | <a href="https://github.com/nfasano/nfasano/blob/main/Fasano_Resume_Current.pdf" target="_blank">Resume</a>
</h3>

____________________________________________________________________________________________

### About me
I am a postdoctoral researcher at Princeton University studying applied physics and actively seeking new career opportunities in data science or quantitative research. I am excited by the prospect of uncovering new insights from vast amounts of data, a skill I developed in the last 6+ years by curating and analyzing massive datasets about light-matter interactions. I am ready to bring my extensive research experience to a mission-driven company where I can apply my technical skills to solve challenging problems.

____________________________________________________________________________________________

### Jump to section
* [Technical Skills](#technical-skills)      
* [Dissertation Research Projects](#dissertation-research-projects)   
* [Data Science Projects](#data-science-projects) 
    * [Sentiment classifier on black lives matter tweets](#1-sentiment-classifier-on-black-lives-matter-tweets-github-repo) 
    * [Content-based movie recommendation system](#2-content-based-movie-recommendation-system-github-repo)
    * [Colosseum ticket tracker and alert system](#3-colosseum-ticket-tracker-and-alert-system-github-repo)  
* [Other Coding Projects](#other-coding-projects) 
    * [Shopping list in Google sheets](#1-shopping-list-in-google-sheets-try-it-here) 
    * [Bash script for executing code through the Slurm scheduler](#2-bash-script-for-executing-code-through-the-slurm-scheduler-github-repo) 
* [Relevant Course Work](#relevant-course-work) 
* [More About Me (Fun/Miscellaneous)](#more-about-me-funmiscellaneous) 

____________________________________________________________________________________________

### Technical skills 
- [x] Python (numpy, pandas, scikit-learn, matplotlib)      
- [x] SQL    
- [x] Matlab    
- [x] Statistical methods and machine learning models
    - [x] Regression (Linear, Multi-linear, Lasso/Ridge, Polynomial, Logistic)
    - [x] Classification (SVM, random forest/decision trees, KNN)
  <!--  - [x] Clustering (K-Means, GMM, Latent Dirichlet Allocation)       -->                        
  <!--  - [x] A/B Testing (Hypothesis Testing) -->
- [x] Data cleaning and preprocessing                                               
- [x] Linux shell scripting  
- [x] High performance computing               
- [x] LaTeX
- [x] Microsoft Word, Excel, and PowerPoint

<!--     - T-test, Anova
    - [x] Time series analysis    -->
____________________________________________________________________________________________

### Dissertation research projects
- [Google scholar profile](https://scholar.google.com/citations?user=X9sdXuQAAAAJ&hl=en) - Link to my publications
- [Thesis](https://github.com/nfasano/nfasano/blob/main/dissertation/Fasano_dissertation_final_compressed.pdf) - Link to view and download my thesis
- [Final public oral slides](https://github.com/nfasano/nfasano/blob/main/dissertation/Fasano_final_public_oral.pdf) - Link to view and download slides from my thesis defense

My dissertation research focused on high-intensity light-matter interactions, where I combined large experimental and numerical datasets to engineer the next generation of short-wavelength, high-power light sources. Devolping these light sources requires advancements in high-power laser science, plasma-based optics, and numerical simulations. 

Main thesis contributions:
- Led an experimental campaign on Princeton's 20TW laser system, which demonstrated waveform-controlled harmonic generation using a novel experimental technique (a multi-pass plasma mirror configuration), resulting in two conference presentations and a written manuscript
- Curated and analyzed terabyte-scale simulation data to show that plasma mirrors are a practical choice for synthesizing and controlling the fundamental properties of intense light sources
- Collaborated with research teams from Lawrence Livermore National Laboratory (LLNL) and the University of Michigan (CUOS group), where I co-designed and executed experiments

<p align="center">
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/DissertationResearchSummary_V2.jpg" alt="drawing" width="900"/> 
</picture>
</p>

_____________________________________________________________________________________________

### Data science projects

#### 1) Sentiment classifier on black lives matter tweets [[Github Repo](https://github.com/nfasano/sentimentClassifier_blmTweets)]  
- **Project description:** Given a dataset of 10,000+ tweets, I built a sentiment classifier to determine whether a given tweet was positive or negative toward the Black Lives Matter (BLM) movement. This work was completed as a course project for COS 524 at Princeton University.
- **Project outcome:** Eight binary classifier models were built to predict whether the sentiment of a tweet was positive or negative toward the Black Lives Matter (BLM) movement. It was found that no model performed significantly better than naively assigning all tweets a positive label (which would yield an accuracy of 81%). Logistic regression achieved the best performance on the held-out test set with an accuracy of 83% and AUC of 0.79, but it was not substantially better than SVM (accuracy = 83%, auc = 0.75) or KNN (accuracy = 83%, AUC = 0.74). Naive Bayes had a low accuracy of 73%, but the highest precision at 92%, suggesting that an ensemble learning model may improve prediction accuracy. Note that chatGPT had an accuracy of 76% on the test dataset without any preprocessing.
- **Skills demonstrated:** Python, pandas, scikit-learn, sentiment analysis, NLP, lemmatization, hypothesis testing, classification models, and evaluation metrics
    
<p align="center">
<picture>
<img src="https://github.com/nfasano/sentimentClassifier_blmTweets/blob/main/images/wordCloud.jpg" alt="drawing" width="700"/> 
</picture>
</p>

*Figure caption: Word clouds for negatively and positively labelled tweets.*

    
#### 2) Content-based movie recommendation system [[Github Repo](https://github.com/nfasano/movie_recsys)]
- **Project description:** Built an end-to-end movie recommendation system, starting with webscraping a set of 150,000+ film scripts and ending with a recommendation app for providing content-based recommendations.
- **Project outcomes:** 
    - Curated a dataset of 150,000+ film scripts through webscraping. Cleaned and synthesized this dataset with relevant metadata collected from publically available datasets (IMDb.com, MovieLens.com, and TMDB.org).
    - Pre-processed the dataset using NLP techniques (e.g. removed stop words, applied lemmatization) and then creates a bag-of-words representation of the entire corpus.
    - Used Latent Dirichlet Allocation to build a topic model, number of topics was chosen based on the calculated perplexity on a held-out test set of movie scripts.  
    - Designed a ranking system by first ordering movies based on topic similarity (cosine-similarity metric) to an input movie and then applying post-processing filters to remove movies below a certain IMDb rating. 
    - Built an app with gradio to provide the top 5 movie recommendations based on a selected movie from the database. I Deployed the app to Hugging Face's spaces ([try it here!](https://nmfasano5-content-based-movie-recommendation-system.hf.space)).
- **Future work:**
    - Extend the movie recommendation system to provide collaborative-based recommendations alongside content-based recommendations. See 'recsys_collab_based' folder in this repository for some examples where I used the MovieLens rating matrix to build and test several models, including a heuristic model (pearson correlation metric), Naive Bayes, and matrix factorization.

- **Skills demonstrated:** Webscraping (beautifulSoup, selenium), SQL, Python, pandas, scikit-learn, NLP, lemmatization, Latent Dirichlet Allocation, gradio

#### 3) Colosseum ticket tracker and alert system [[Github Repo](https://github.com/nfasano/colosseumTickets)]
- **Project description:** Wrote an algorithm to track the ticket availability for entry into the Colosseum from the official website ([Coopculture](https://ecm.coopculture.it/index.php?lang=en)), where tickets are notoriously difficult to secure. Ticket availability was queried for 14 consecutive days in intervals between 3 seconds and one minute, depending on the time of day. Based on the collected data, a detailed plan is proposed to ensure that you get the best available tickets. Other features of the code allow for the user to be sent instantaneous email alerts with embedded links when tickets become available.
- **Skills demonstrated:** Webscraping, pandas, data visualization, data cleaning and processing
_____________________________________________________________________________________________

### Other coding projects

#### 1) Shopping list in Google sheets [[Try it here](https://docs.google.com/spreadsheets/d/1JmDtCFYWc8K8Y4g38fVQvjgUsC7UjRVS25mL4au47Pw/edit?usp=sharing)]
- **Project description:** Created a shopping list which automatically arranges selected items in the order that one walks through the store, making my shopping trips more efficient. Features include crossing off items with checkboxes, removing checked items, all items, or a single item by clicking a checkbox. Convenient addition of items using a searchable dropdown list. Future features will include pricing an aisle information from webscraped data and the ability to add entire recipes with one click.
- **Skills demonstrated:** google sheets, JavaScript programming 

#### 2) Bash script for executing code through the Slurm scheduler [[Github Repo](https://github.com/nfasano/bashScriptsHPC)]
- **Description:** Wrote a bash script that submits batches of simulations with different parameters and requested computational resources to the Slurm scheduler (a commonly used cluster management and job scheduling system for HPC clusters). This script provides an organized framework for managing massively parallel simulations and terabyte-scale datasets and has been adopted by successive graduate students who use the HPC cluster in a myriad of ways.
- **Skills demonstrated:** Linux shell scripting, High performance computing 

<!-- - **Ray tracing renderer ** - (Github Repo)
    - Description: Following the "Ray Tracing in One Weekend" series by Peter Shirley, I implemented a functioning ray tracing algorithm capable of rendering spheres, boxes, triangles with the option for different textures.
    - Skills demonstrated: C++, object oriented programming -->
_____________________________________________________________________________________________

### Relevant course work:
#### Princeton University (Graduate level courses):
- **ELE 535: Machine Learning and Pattern Recognition** - A variety of classical and recent results in theoretical machine learning and statistical analysis were discussed, including: Bayesian classification, regression, regularization, SVD, PCA, support vector machines, kernels, neural networks and gradient descent.
- **COS 524: Fundamentals of Machine Learning** (audited - no credit given, but see projects above) - This course focused on useful approaches to analyzing large complex data sets, exploring both theoretical foundations and practical applications of machine learning. Course covered classification, regression, clustering, dimension reduction (PCA, SVD, NNMF, LDA) and time series models.
- **MAE 501: Mathematical Methods of Engineering Analysis I** - Covered mathematical topics in linear algebra, matrices, eigenvalue problems, and ordinary and partial differential equations.
#### Online course work:
- **Andrew Ng’s Deep Learning Specialization** | Coursera | [Credential URL](https://www.coursera.org/verify/specialization/GA9QPDNUG6RB)
- **Python for Data Science and Machine Learning Bootcamp** | Udemy | [Credential URL](https://www.ude.my/UC-457a4c2d-3129-4238-b3b9-c476db07faad/)

_____________________________________________________________________________________________

### More about me (Fun/Miscellaneous)
- I am a home cook who loves experimenting with new recipes and flavors from all cuisines
- I enjoy the art of photography, both for the journey of capturing the photo and for understanding the story that the photo tells

<!-- - ⚡ Fun fact about me: I made a grand entrance into the world by being born "en caul", a condition where a baby is delivered inside a fully intact amniotic sac. According to some cultures, this is considered a sign of good luck and it's also believed that babies born en caul are incapable of drowning. So, let's just say I'm a lucky and unsinkable little bundle of joy!"
-->
<p align="center">
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/2020_06_02_DSC_0133_4x6Print.jpg" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_0216_4x6Print.jpg" alt="drawing" width="250"/>
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_0346_V3.png" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_1157_Cropped.jpg" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_0411_TouchUp.jpg" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/BuffaloChickenPizza_4x6.jpg" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/IMG_3527_2f.jpg" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/IMG_3533_2.jpg" alt="drawing" width="250"/> 
</picture>
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/Ramen_22.jpg" alt="drawing" width="250"/> 
</picture>
</p>



<!--
**nfasano/nfasano** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 
- 😄 Pronouns: ...

-->
