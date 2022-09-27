# eBimPy project

The present work has been carried out to solve a challenge provided by the Institute of Technology Rakuten (https://challengedata.ens.fr/challenges/35) and aims at developing an efficient supervised hybrid Deep Learning / Machine Learning model for the classification of large-scale product listings into product type codes through text and image. 
For this challenge Rakuten has provided a dataset containing roughly 85k labeled products (the train set) and 14k non labeled ones (the test set) as defined by the Rakuten France catalog. Each product is identified by a product id and image id. This latter connects the products to their corresponding images from a zip folder. The datasets contain the following features: 
*	designation of type string containing the product title and a short text about the product
*	description of type string including a more detailed description of the product
*	productid of type integer that is a unique ID for each product
*	imageid of type integer that is a unique ID for the image associated with the product

Given a new set of non-labeled items (test set), the objective is to correctly assign a prdtype code to each of them. In order to perform such classification task, the project has been divided into three main parts:
1.	Text classification: the text features designation and description have been leveraged to train a Machine Learning and a Deep Learning model eventually used to predict the prdtypecode
2.	Image classification: the images associated to each product have been employed to train a Deep Learning algorithm  eventually used to predict the prdtypecode
3.	Image and text classification: two hybrid Deep Learning / Machine learning models has been devised and trained on both text and image in order to predict the prdtypecode

Several models for text and image classification have been tested and compared through an accurate qualitative and quantitative analysis by means of the accuracy, recall, precision and f1 metrics and the best ones have been employed to devise the mixed final Deep Learning / Machine Learning model. 

The work has been organized in different notebooks according to the following tasks:
1.	Text Classification by Machine Learning
2.	Text Classification by Deep Learning
3.	Image Classification by Deep Learning
4.	Hybrid Text and Image Classification
