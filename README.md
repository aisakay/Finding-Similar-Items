[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aisakay/Finding-Similar-Items/blob/main/notebooks/Finding_Similar_Items_100K.ipynb)

# Finding-Similar-Items
The task is to implement a detector of pairs of similar abstract for scientific papers, using the abstract field in the arXiv dataset, published under the Public Domain license.
# Abstract
 This project of Finding Similar Items is a detector to build similar abstracts from the kaggle
dataset of arXiv articles that contains more than 3 million articles. To encode abstracts 3-word
shingling was chosen, similarity was measured using Jaccard similarity and two techniques
from the course were used, namely, MinHashing and LSH (Local Sensitivity Hashing). The
beginning 100,000 rows of dataset was preprocessed and analyzed. Scalability is also explored
by implementing the code on inital 500,000 rows of dataset. For 100K rows 1227 candidate
pairs were identified using LSH and 611 had Jaccard similarity above the threshold of 0.5. MAE
was equal to 0.02495. The results of this experiment show a significant reduction of pairs to be
compared thanks to smaller candidates’ pool found by LSH.
