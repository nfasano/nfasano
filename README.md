<h3 align="center">
    Nicholas Fasano
</h3>
<h3 align="center">
    nmfasano5@gmail.com | <a href="https://www.linkedin.com/in/nmfasano/" target="_blank">LinkedIn</a> | <a href="https://github.com/nfasano/nfasano/blob/main/Fasano_Resume.pdf" target="_blank">Resume</a>
</h3>

____________________________________________________________________________________________
### About me

I am an applied scientist at Princeton University looking for data science opportunities at mission-driven companies where I can leverage my technical experience, problem-solving capabilities, and collaborative nature to find innovative solutions that address real-world problems.

I have six years of experience leading data-driven research projects on developing advanced ultraviolet and X-ray light sources for potential applications in biology, medicine, material science, and fundamental physics. I have presented the key findings of my research at leading technical conferences and in peer-reviewed journals. 

Beyond my own research, I have collaborated on interdisciplinary projects with several responsibilities, including high-level project planning, data collection, analysis and interpretation of results, and mentoring of undergraduate and graduate student researchers.

Outside the lab, my passion for education led me to enroll in the Teaching Transcript Program offered by Princeton's McGraw Center for Teaching and Learning. In this program, I taught for six semesters and participated in several pedagogy workshops where I engaged in discussions to learn and develop strategies that improve student learning. The program culminated with me writing an original course syllabus and a teaching philosophy statement, for which I received a teaching certificate from the McGraw Center.

Moving forward, I am committed to staying at the forefront of data science and technology trends so that I can continue to solve challenging problems and effectively communicate my findings to stakeholders and collaborators.
____________________________________________________________________________________________

### Jump to section
* [Technical skills](#technical-skills)      
* [Dissertation research projects](#dissertation-research-projects)   
* [Data science projects (with write-ups)](#data-science-projects)
    * [Enhanced movie recommendations using a collaborative topic model](#1-enhanced-movie-recommendations-using-a-collaborative-topic-model)
    * [A data-backed approach for securing tickets to see Rome's Colosseum](#2-a-data-backed-approach-for-securing-tickets-to-see-romes-colosseum)  
    * [Sentiment classifier on black lives matter tweets](#3-sentiment-classifier-on-black-lives-matter-tweets) 
* [Other coding projects](#other-coding-projects) 
    * [Shopping list in Google sheets](#1-shopping-list-in-google-sheets) 
    * [Bash script for executing code through the Slurm scheduler](#2-bash-script-for-executing-code-through-the-slurm-scheduler) 
* [Relevant course work](#relevant-course-work) 
* [More about me (fun/miscellaneous)](#more-about-me-funmiscellaneous) 

____________________________________________________________________________________________

### Technical skills 
- [x] Python (numpy, pandas, scikit-learn, matplotlib)      
- [x] SQL    
- [x] Matlab    
- [x] Statistical methods and machine learning models
    - [x] Regression (Linear, Lasso/Ridge)
    - [x] Classification (Logistic, decision trees, KNN)
    - [x] Unsupervised (SVD, PCA, k-means, Latent Dirichlet Allocation)
    - [x] A/B Testing (Hypothesis Testing) 
  <!--  - [x] Clustering (K-Means, GMM, Latent Dirichlet Allocation)       -->                        
  <!--   -->
- [x] Data cleaning and preprocessing                                               
- [x] Linux shell scripting  
- [x] High-performance computing               
- [x] LaTeX

<!--     - T-test, Anova
    - [x] Time series analysis    -->
____________________________________________________________________________________________

### Dissertation research projects
- [Google scholar profile](https://scholar.google.com/citations?user=X9sdXuQAAAAJ&hl=en) - Link to my publications
- [Thesis](https://github.com/nfasano/nfasano/blob/main/dissertation/Fasano_dissertation_final_compressed.pdf) - Link to view and download my thesis
- [Final public oral slides](https://github.com/nfasano/nfasano/blob/main/dissertation/Fasano_final_public_oral.pdf) - Link to view and download slides from my thesis defense

My dissertation research focused on high-intensity light-matter interactions, where I combined large experimental and numerical datasets to engineer the next generation of short-wavelength, high-power light sources. Developing these advanced light sources requires advancements in high-power laser science, massively parallel simulations, and plasma-based optics.

<picture> <img src="https://github.com/nfasano/nfasano/blob/main/images/DissertationResearchSummary_V2.jpg" alt="drawing" width="100%"/> </picture> 

Main thesis contributions:
- Curated and wrangled terabyte-scale simulation data on a high-performance computing cluster to build models of the ultraviolet and X-ray light sources generated in laser-plasma interactions
- Utilized python (numpy and scikit-learn) to model the data with linear regression, identifying parameter regimes that optimize the energy in ultraviolet and X-ray light sources
- Spearheaded the data collection and analysis of an experimental campaign which demonstrated a statistically significant 1.6x increase in ultraviolet light energy when using a 2-color laser instead of a 1-color laser
- Presented key research findings at six technical conferences and in two peer-reviewed journal articles
- Collaborated with teams at national labs and universities, contributing to data analysis and experiment execution
- Mentored undergraduate and graduate students on their research projects, covering topics in solid-state harmonic generation, interaction of lasers with ultrathin (nm-scale) plasmas, and laser-brewed coffee

_____________________________________________________________________________________________

### Data science projects

#### 1) Enhanced movie recommendations using a collaborative topic model 
- [GitHub Repo](https://github.com/nfasano/movie_recsys)
- **Project description:** Inspired by the seductive power of Tik-Tok's personalized feed and a strong desire to learn how industry recommender systems are designed, I developed an end-to-end movie recommender system. The recommender model is based on the Collaborative Topic Model (CTM), a hybrid approach that combines topic information from film scripts and user-movie interactions from a ratings matrix. This hybrid model achieves a modest (1%) improvement in root-mean-square error compared to traditional matrix factorization approaches, but alleviates the item cold-start problem thanks to the topic model. Finally, I deployed the recommender as a web-based app on Hugging Face Spaces for anyone to demo.

 [Get your movie recommendation here!](https://nmfasano5-content-based-movie-recommendation-system.hf.space)
- **Project outcomes:** 
    - Engineered a data pipeline for web-scraping, cleaning, and processing 160k film scripts using NLP. Synthesized film scripts with external datasets (IMDb and MovieLens) into a database that can be queried with SQL
    - Processed the film scripts dataset using NLP techniques, including stop word removal and lemmatization, and then created a bag-of-words representation for the corpus
    - Built a collaborative topic model (latent Dirichlet allocation + SVD) that shows a modest (1%) improvement in RMSE compared to SVD alone, but alleviates the new item cold-start problem with a recall@20 score of 41% for unrated movies
    - To serve the recommendations, I built a web-based app using gradio and deployed it to Hugging Face's Spaces. The app returns the recommendations, ranked according to cosine-similarity between the movies latent topics, along with IMDb metadata (genre, IMDb rating, IMDb link) and poster art from tmdb.org.
- **Future work:**
    - Build word and image embeddings using film scripts and movie posters, respectively, and build a ranking model based on the two-tower architecture
- **Skills demonstrated:** Webscraping (beautifulSoup, selenium), SQL, Python, pandas, scikit-learn, NLP, lemmatization, Latent Dirichlet Allocation, SVD, Gradio

____________________________________________________________________________________________

#### 2) A data-backed approach for securing tickets to see Rome's Colosseum 
- [GitHub Repo](https://github.com/nfasano/colosseum_ticket_tracker)
- **Project description:** Wrote an algorithm to track the ticket availability for entry into the Colosseum from the official website ([Coopculture](https://ecm.coopculture.it/index.php?lang=en)), where tickets are notoriously difficult to secure. Ticket availability was queried for 14 consecutive days in intervals between 3 seconds and one minute, depending on the time of day. Based on the collected data, a detailed plan is proposed to ensure that you get the best available tickets. Other features of the code allow for the user to be sent instantaneous email alerts with embedded links when tickets become available.
- **Skills demonstrated:** Webscraping, pandas, data visualization, data cleaning and processing

____________________________________________________________________________________________

#### 3) Sentiment classifier on black lives matter tweets 
- [GitHub Repo](https://github.com/nfasano/sentiment_classifier_blm_tweets)
- **Project description:** Given a dataset of 10,000+ tweets, I built a sentiment classifier to determine whether a given tweet was positive or negative toward the Black Lives Matter (BLM) movement. This work was completed as a course project for COS 524 at Princeton University.
- **Project outcome:** Eight binary classifier models were built to predict whether the sentiment of a tweet was positive or negative toward the Black Lives Matter (BLM) movement. It was found that no model performed significantly better than naively assigning all tweets a positive label (which would yield an accuracy of 81%). Logistic regression achieved the best performance on the held-out test set with an accuracy of 83% and AUC of 0.79, but it was not substantially better than SVM (accuracy = 83%, auc = 0.75) or KNN (accuracy = 83%, AUC = 0.74). Naive Bayes had a low accuracy of 73%, but the highest precision at 92%, suggesting that an ensemble learning model may improve prediction accuracy. Note that chatGPT had an accuracy of 76% on the test dataset without any preprocessing.
- **Skills demonstrated:** Python, pandas, scikit-learn, sentiment analysis, NLP, lemmatization, hypothesis testing, classification models, and evaluation metrics
    
<picture> <img src="https://github.com/nfasano/sentimentClassifier_blmTweets/blob/main/images/wordCloud.jpg" alt="drawing" width="80%"/> </picture> 

*Figure caption: Word clouds for negatively and positively labelled tweets.*
_____________________________________________________________________________________________

### Other coding projects

#### 1) Shopping list in Google sheets 
- [Try it here](https://docs.google.com/spreadsheets/d/1JmDtCFYWc8K8Y4g38fVQvjgUsC7UjRVS25mL4au47Pw/edit?usp=sharing)
- **Project description:** Created a shopping list that automatically arranges selected items in the order that one walks through the store, making anyone's shopping experience more efficient. Features include adding items to the list using a searchable dropdown list, crossing off items on the list with checkboxes, and removing a single item or all items by clicking a checkbox. Future features will include pricing and aisle information from web-scraped data as well as the ability to add entire recipes with one click.
- **Skills demonstrated:** google sheets, JavaScript programming 

#### 2) Bash script for executing code through the Slurm scheduler 
- [GitHub Repo](https://github.com/nfasano/bash_scripts_for_hpc)
- **Description:** Wrote a bash script that submits batches of simulations with different parameters and requested computational resources to the Slurm scheduler (a commonly used cluster management and job scheduling system for HPC clusters). This script provides an organized framework for managing massively parallel simulations and terabyte-scale datasets and has been adopted by successive graduate students who use the HPC cluster in a myriad of ways.
- **Skills demonstrated:** Linux shell scripting, High-performance computing 
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

### More about me (fun/miscellaneous)
- I am a home cook who loves experimenting with new recipes and flavors from all cuisines
- I enjoy the art of photography, both for the journey of capturing the photo and for understanding the story that the photo tells

<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/2020_06_02_DSC_0133_4x6Print.jpg" alt="drawing" width="32%"/></picture>
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_0216_4x6Print.jpg" alt="drawing" width="32%"/></picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_0346_V3.png" alt="drawing" width="32%"/> </picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_1157_Cropped.jpg" alt="drawing" width="32%"/> </picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/DSC_0411_TouchUp.jpg" alt="drawing" width="32%"/> </picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/BuffaloChickenPizza_4x6.jpg" alt="drawing" width="32%"/> </picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/IMG_3527_2f.jpg" alt="drawing" width="32%"/> </picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/IMG_3533_2.jpg" alt="drawing" width="32%"/> </picture> 
<picture><img src="https://github.com/nfasano/nfasano/blob/main/images/Ramen_22.jpg" alt="drawing" width="32%"/> </picture> 

