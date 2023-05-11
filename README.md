<h3 align="center">
    Nicholas Fasano
</h3>
<h3 align="center">
    nmfasano5@gmail.com | <a href="https://www.linkedin.com/in/nmfasano/" target="_blank">LinkedIn</a> | <a href="https://github.com/nfasano/nfasano/blob/main/Fasano_Resume_Current.pdf" target="_blank">Resume</a>
</h3>

____________________________________________________________________________________________

### About me
I am a Ph.D. candidate studying applied physics at Princeton University, graduating in May, and actively seeking new career opportunities in data science or quantitative research. I am excited by the prospect of uncovering new insights from vast amounts of data, a skill I developed in the last 5+ years by curating and analyzing massive datasets about light-matter interactions. I am ready to bring my extensive research experience to a mission-driven company where I can apply my technical skills to solve challenging problems.

____________________________________________________________________________________________

### Jump to section: 
* [Technical Skills](#technical-skills)      
* [Dissertation Research Projects](#dissertation-research-projects)   
* [Data Science Projects](#data-science-projects) 
    * [1) Sentiment classifier on black lives matter tweets](1-sentiment-classifier-on-black-lives-matter-tweets) 
    * [2) Movie Recommendation System (In progress)](#2-movie-recommendation-system-in-progress) 
* [Other Coding Projects](#other-coding-projects) 
    * [1) Sentiment classifier on black lives matter tweets](1-sentiment-classifier-on-black-lives-matter-tweets) 
    * [2) Movie Recommendation System (In progress)](#2-movie-recommendation-system-in-progress) 
    * [2) Movie Recommendation System (In progress)](#2-movie-recommendation-system-in-progress) 
* [Relevant Course Work](#relevant-course-work) 
* [More About Me (Fun/Miscellaneous)](#more-about-me-funmiscellaneous) 

____________________________________________________________________________________________

### Technical Skills 
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

### Dissertation Research Projects: 
[Google scholar profile](https://scholar.google.com/citations?user=X9sdXuQAAAAJ&hl=en)

My dissertation research focused on high-intensity light-matter interactions, where I combined large experimental and numerical datasets to engineer the next generation of short-wavelength, high-power light sources. Devolping these light sources requires advancements in high-power laser science, plasma-based optics, and numerical simulations. 

Main Thesis Contributions:
- Led an experimental campaign on Princeton's 20TW laser system, which demonstrated waveform-controlled harmonic generation using a novel experimental technique (a multi-pass plasma mirror configuration), resulting in two conference presentations and a written manuscript
- Curated and analyzed terabyte-scale simulation data to show that plasma mirrors are a practical choice for synthesizing and controlling the fundamental properties of intense light sources
- Collaborated with research teams from Lawrence Livermore National Laboratory (LLNL) and the University of Michigan (CUOS group), where I co-designed and executed experiments

<p align="center">
<picture>
<img src="https://github.com/nfasano/nfasano/blob/main/images/DissertationResearchSummary_V2.jpg" alt="drawing" width="900"/> 
</picture>
</p>

_____________________________________________________________________________________________

### Data Science Projects:

#### 1) Sentiment classifier on black lives matter tweets    
- [Github Repo](https://github.com/nfasano/sentimentClassifier_blmTweets)
- **Project Description:** Given a dataset of 10,000+ tweets, I built a sentiment classifier to determine whether a given tweet was positive or negative toward the Black Lives Matter (BLM) movement. This work was completed as a course project for COS 524 at Princeton University.
- **Project Outcome:** It was found that no model performed significantly better than a naively assigning all tweets a positive label (which would yield an accuracy of 80%). Logistic regression achieved the best performance on the held out testing with an accuracy of 83% and AUC of 0.79, but it was not substantially better than SVM (accuracy = 83%, auc = 0.75) or KNN (accuracy = 83%, AUC = 0.74). Naive Bayes had a low accuracy of 73%, but the highest precision of 92%, suggesting that an ensemble learning model may improve predcition accuracy.
- **Skills Demonstrated:** Python, sentiment analysis, NLP, hypothesis testing, classification models and evaluation metrics
    
<p align="center">
<picture>
<img src="https://github.com/nfasano/sentimentClassifier_blmTweets/blob/main/images/wordCloud.jpg" alt="drawing" width="900"/> 
</picture>
</p>
<!-- - **Predicting Fragile Family Outcomes** (Github Repo)
    - Project Description:
    - Skills Demonstrated:  -->
    
#### 2) Movie recommendation system (in progress) 
- [Github Repo](https://github.com/nfasano/movieScripts) 
- **Project Description:** Given a set of 160,000+ movie/show scripts, titles, genres, cast/crew, ratings, budget, earnings, etc., I aim to build a movie recommendation system using a topic model (Latent Dirichlet Allocation). 
- **Project Outcomes:** 
    - Curated a dataset containing 30,000+ movie scripts and 130,000+ TV episode scripts through webscraping
    - Combined movie script data with dataset available from IMDb.com containing pertinent movie/show information (e.g. ratings, cast/crew, genre, etc.)
- **Skills Demonstrated:** Webscraping (beautifulSoup, selenium), SQL, NLP, Latent Dirichlet Allocation,  

_____________________________________________________________________________________________

### Other Coding Projects:

#### 1) Colosseum ticket tracker and alert system
- [Github Repo](https://github.com/nfasano/colosseumTickets)
- **Description:** Wrote an algorithm to track the ticket availability on the official Colosseum website ([Coopculture](https://ecm.coopculture.it/index.php?option=com_snapp&view=products&snappTemplate=template3&catalogid=ADAE8874-AE4B-55B9-02FB-0167A81C0247&lang=en)), where tickets are notoriously difficult to secure. Ticket information was queried in intervals between 5 seconds and one minute, depending on the time of day. Based on this information, a detailed plan is proposed to ensure that you get the best available tickets. Other features of the code allow for the user to be updated by email when tickets for a particular date go on sale.
- **Skills demonstrated:** Webscraping, pandas

#### 2) Bash script for executing code through the Slurm scheduler 
- [Github Repo](https://github.com/nfasano/bashScriptsHPC)
- **Description:** Wrote a bash script that submits batches of simulations with different parameters and requested computational resources to the Slurm scheduler (a commonly used cluster management and job scheduling system for HPC clusters). This script provides an organized framework for managing massively parallel simulations and terabyte-scale datasets and has been adopted by successive graduate students who use the HPC cluster in a myriad of ways.
- **Skills demonstrated:** Linux shell scripting, High performance computing 

#### 3) Shopping list in Google sheets 
- [Try it Here](https://docs.google.com/spreadsheets/d/1JmDtCFYWc8K8Y4g38fVQvjgUsC7UjRVS25mL4au47Pw/edit?usp=sharing)
- **Description:** Created a shopping list which automatically arranges selected items in the order that one walks through the store, making my shopping trips more efficient. Features include crossing off items with checkboxes, removing checked items, all items, or a single item by clicking a checkbox. Convenient addition of items using a searchable dropdown list. Future features will include pricing an aisle information from webscraped data and the ability to add entire recipes with one click.
- **Skills demonstrated:** google sheets, JavaScript programming 

<!-- - **Ray tracing renderer ** - (Github Repo)
    - Description: Following the "Ray Tracing in One Weekend" series by Peter Shirley, I implemented a functioning ray tracing algorithm capable of rendering spheres, boxes, triangles with the option for different textures.
    - Skills demonstrated: C++, object oriented programming -->
_____________________________________________________________________________________________

### Relevant Course Work:
#### Princeton University (Graduate Level Courses):
- **ELE 535: Machine Learning and Pattern Recognition** - A variety of classical and recent results in theoretical machine learning and statistical analysis were discussed, including: Bayesian classification, regression, regularization, SVD, PCA, support vector machines, kernels, neural networks and gradient descent.
- **COS 524: Fundamentals of Machine Learning** (audited - no credit given, but see projects above) - This course focused on useful approaches to analyzing large complex data sets, exploring both theoretical foundations and practical applications of machine learning. Course covered classification, regression, clustering, dimension reduction (PCA, SVD, NNMF, LDA) and time series models.
- **MAE 501: Mathematical Methods of Engineering Analysis I** - Covered mathematical topics in linear algebra, matrices, eigenvalue problems, and ordinary and partial differential equations.
#### Online Course Work:
- **Andrew Ng’s Deep Learning Specialization** | Coursera | [Credential URL](https://www.coursera.org/verify/specialization/GA9QPDNUG6RB)
- **Python for Data Science and Machine Learning Bootcamp** | Udemy | [Credential URL](https://www.ude.my/UC-457a4c2d-3129-4238-b3b9-c476db07faad/)

_____________________________________________________________________________________________

### More about me (Fun/Miscellaneous):
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
