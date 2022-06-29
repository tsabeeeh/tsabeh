# Detect Plant Disease Using fast.ai

Introduction:

Creating an AI web application that detects diseases in plants using FastAi which built on the top of Facebook’s deep learning platform: PyTorch. According to the Food and Agriculture Organization of the United Nations (UN), transboundary plant pests and diseases affect food crops, causing significant losses to farmers and threatening food security.

# Motive
For this challenge, I used the “PlanVillage” dataset. This dataset contains an open access repository of images on plant health to enable the development of mobile disease diagnostics. The dataset contains 54, 309 images. The images span 14 crop species: Apple, Blueberry, Cherry, Grape, Orange, Peach, Bell Pepper, Potato, Raspberry, Soybean, Squash, Strawberry, and Tomato. It contains images of 17 fundal diseases, 4 bacterial diseases, 2 molds (oomycete) diseases, 2 viral diseases, and 1 disease caused by a mite. 12 crop species also have images of healthy leaves that are not visibly affected by a disease.
I have used Google Cloud Platform with the base platform called, n1-highmem-8, and costs $0.12 per hour. Attaching a P4 GPU costs $0.26 per hour so both together amount to $0.38 per hour. And the suggested 200GB Standard Disk storage size, there will be an additional charge of $9.60 a month. For a full walkthrough, setup visit here!

# Training
I have used fastai which is built on top of Pytorch. Dataset consists of 38 disease classes from PlantVillage dataset and 1 background class from Stanford’s open dataset of background images DAGS. 80% of the dataset is used for training and 20% for validation.
We will use the pre-trained resnet34 model to solve the issue with the training

