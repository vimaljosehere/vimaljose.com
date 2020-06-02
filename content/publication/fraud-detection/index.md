---
title: "Fraud Detection through Deep User Representations and Single Class learning with Generative Adversarial Networks (GANs)"
authors:
- admin
date: "2020-02-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["7"]

# Publication name and optional abbreviated publication name.
publication: In *Liverpool John Moores University school of Computer Science*
publication_short: In *LJMU school of CS*

abstract: As the reach and role of internet increases in our daily lives, the impact of internet frauds on our lives increases exponentially. With most of our transactions being made online – from transferring money to making friends and from acquiring knowledge to finding a romantic partner – there is no limit for the impact and effect of online frauds. And the same is applicable more so for businesses and establishments as internet frauds often result in monetary and non-monetary losses to businesses including their credibility and goodwill. A few examples for these are – the spread of fake news on social media, dissemination of fake information on knowledge sharing platforms like Wikipedia, fake profiles on social media platforms and fraudulent transactions in financial networks. Even though this has been well researched before, two of the major challenges that hold us back from eradicating them completely are:
1. The percentage of reported or identified malicious activity among the total user behavior is very small. For e.g., the reported % of fraud transactions in total payments in the US for 2016 is 0.0014%. [28][29]
2. Once a pattern of fraud is starting to be detected by the security systems, the attackers malicious agents change their pattern.
3. Waiting long enough to collect the required amount of data for detection often ends up being too late.
To specify the same in machine learning terms, this means the non-availability of enough data for the fraud classes is one of the key reasons why the current systems are unable to detect malicious activity early enough.
Another key point is that in most of the online malicious activities, it has been noticed that most of them contains repetitive factors – be it in terms of users, associations, history and repeated patterns of transactions. So, it can be said that knowing the history and the associations of the users / actors involved might be an important factor in detecting fraud. In other words, fraud detection is more effective if done at a user level than at a transaction level. So, it is important that fraud detection needs to be done in a stateful manner at the actor level. To specify the same in machine learning terminology, and ideal fraud detection algorithm should be a sequence classifier rather than a data point classifier.
Keeping these in mind, the goal this paper is to build a detection algorithm which can:
1. Detect without any data regarding the fraudulent activity beforehand.
2. Identify new patterns of fraud even when we have no previous data to learn from.
3. Make use of the history of an actor when available.
Based on these goals, the proposed approach in this paper is to build a one-class classifier (OCC) for non-fraud users. We’ll be making use of an LSTM-autoencoder to convert the actor history, whenever available into user representations in a fixed dimensional feature space. These user representations will be used for generating the user representations of malicious users by a complimentary GAN generator and the GAN discriminator will be used as one of the final classifiers.
For testing these assumptions, we will be working on the Wikipedia edits dataset for identifying Wikipedia Vandalism. So the goal of this research would be to develop a system using LSTM auto encoder and a complimentary GAN to correctly identify wikipedia vandals based on the Wikipedia Edits dataset.

# Summary. An optional shortened abstract.
summary: The proposed approach in this paper is to build a one-class classifier (OCC) for non-fraud users. We’ll be making use of an LSTM-autoencoder to convert the actor history, whenever available into user representations in a fixed dimensional feature space. These user representations will be used for generating the user representations of malicious users by a complimentary GAN generator and the GAN discriminator will be used as one of the final classifiers.

tags:
- Fraud Detection
- GAN
- LSTM
- OCC
featured: true

links:
- name: Custom Link
  url: http://example.org
url_pdf: Fraud_Detection.pdf
url_code: '#'
url_dataset: '#'
url_poster: '#'
url_project: ''
url_slides: ''
url_source: '#'
url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

