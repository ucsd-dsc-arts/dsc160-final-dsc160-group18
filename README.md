# Project Title

DSC160 Data Science and the Arts - Final Project - Generative Arts - Spring 2020

Project Team Members: 
- Brian Qian - brqian@ucsd.edu 

- Emma Logomasini - elogomas@ucsd.edu 

- Nicholas Kho - nikho@ucsd.edu 

## Abstract

In our Midterm project, our team looked at important songs of each era as outlined in the Sogang University's Professor Huikyong Pang’s class “The Mediums of Korean Cultural Modernity.” We attempted to analyze political periods in association with music trends; however, our analysis was limited by the size of our dataset and our choices in analytical techniques. We are still interested in music over time in Korea, but instead this project will be focusing on the visual aspect of korean music specifcally the album art. 

Since K-pop music albums are often strongly associated with its visual branding and concept, we believe it would be interesting to look at album covers from top K-pop albums to new generate concepts with (to clarify, the definition we are using for “K-pop” refers to Korean “idol music” as opposed to all Korean pop songs). For this dataset, we plan on using the Gaon Album Chart data to find the top-selling albums for the 2010s. 

Our first exploration will be a focused on generating album art based on the top selling albums of recent korean history. We then want to explore different datasets of album art from popular boy groups, girl groups, and their icons/logos, to see the constrating or similar aspects of each demographic. Finally we will scrap random kpop album art from Google and Bing to have a more generalized and larger dataset to generate album art from, also to see how different general kpop album covers are from popular kpop albums. In short, our project will provide greater insight into visual aspects of what makes a popular korean album in conjunction with specific categories like girl groups and boy groups.

To achieve all of this, our technical process will include the use of jupyterhub while utilizing numerous libraries including TensorFlow, Pillow, Keras, and scikit-learn to recreate a deep covolutional generative adversarial network (DCGAN) that will help us process new album art and display our results in jpg format. 


## Data and Model

Our main training data is from the Gaon Album Chart, Korea’s national music chart, and every year since 2010 they provide a top 10 list of the best-selling albums of the entire year. Gaon’s ranking process revolves around compiling domestic shipments in weekly, monthly, and year-end formats to which we will utilize their year-end charts.The album cover images will be collected from Melon, Korea's top streaming service, to have accurate digital images of the respective albums in their native country. [Link to Gaon Album Chart Data](https://en.wikipedia.org/wiki/Gaon_Album_Chart)

Since our main dataset is limited by the size of around 100 popular covers, for additional exploration purposes we will also collect a different generalized/larger dataset by scrapping random kpop album art from Google and Bing to further generate new album covers from. To achieve this, we will be utilizing the icrawler python library and input english and korean keywords such as ‘kpop album art’ to download around 500 random covers. [Link to icrawler library](https://developer.aliyun.com/mirror/npm/package/icrawler).

Our generative adversarial model is based on MLWhiz’s DC-GAN architecture to which they generated new anime characters from. The idea behind the GAN originated from the paper, [“Unsupervised Representation Learning With Deep Convolutional Generative Adversarial Network”](https://arxiv.org/pdf/1511.06434.pdf) by Alex Radford, Luke Metz, and Soumith, where they discussed how the two main components were a generator and a discriminator. [Link to MLWhiz](https://mlwhiz.com/blog/2019/06/17/gans/).


## Code

[Scrapping Code File](code/scrapper.ipynb)

For the data acquistion portion of our code, we first utilized icrawler's 

[Preprocessing & Neural Network Code File](code/network.ipynb)

For the analysis portion of our code, 

(20 points)

This section will link to the various code for your project (stored within this repository). Your code should be executable on datahub, should we choose to replicate your result. This includes code for: 

- code for data acquisition/scraping
- code for preprocessing
- training code (if appropriate)
- generative methods

Link each of these items to your .ipynb or .py files within this seection, and provide a brief explanation of what the code does. Reading this section we should have a sense of how to run your code.

## Results

(30 points) 

This section should summarize your results and will embed links to documentation to significant outputs. This should document both process and show artistic results. This can include figures, sound files, videos, bitmaps, as appropriate to your generative art idea. Each result should include a brief textual description, and all should be listed below: 

- image files (`.jpg`, `.png` or whatever else is appropriate)
- audio files (`.wav`, `.mp3`)
- written text as `.pdf`

## Discussion

(30 points, three to five paragraphs)

The first paragraph should be a short summary describing your results.

The subsequent paragraphs could address questions including:
- Why is this culturally innovative?
- How does your generative computational approach differ from traditional art/music/cultural production? 
- How do your results relate to broader social, cultural, economic political, etc., issues? 
- What are the ethical concerns for this form of generative art? 
- In what future directions could you expand this work?

## Team Roles

Provide an account of individual members and their efforts/contributions to the specific tasks you accomplished.

## Technical Notes and Dependencies

Any implementation details or notes we need to repeat your work. 
- Additional libraries you are using for this project
- Does this code require other pip packages, software, etc?
- Does this code need to run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

https://towardsdatascience.com/generating-modern-arts-using-generative-adversarial-network-gan-on-spell-39f67f83c7b4

https://towardsdatascience.com/cyclegans-to-create-computer-generated-art-161082601709

https://heartbeat.fritz.ai/stylegans-use-machine-learning-to-generate-and-customize-realistic-images-c943388dc672

https://towardsdatascience.com/dcgans-generating-dog-images-with-tensorflow-and-keras-fb51a1071432


https://mlwhiz.com/blog/2019/06/17/gans/

https://www.researchgate.net/publication/318987126_Album_Cover_Generation_from_Genre_Tags

https://machinelearningmastery.com/what-are-generative-adversarial-networks-gans/

