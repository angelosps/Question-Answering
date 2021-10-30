# Question Answering❓

Fine-Tuning BERT for contextual Question Answering. That is, given a context (passage) in the model, it predicts a start and an end position in the passage that answers the particular question. More specifically, I fine-tune the `bert-base-uncased` model on the [Stanford Question Answering Dataset (SQuAD) 2.0](https://rajpurkar.github.io/SQuAD-explorer/).

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WxGxCFE_1cESJ02baaBY-HBHmGjSlxJx?usp=sharing) 

An example of question answering on a passage about Athens.

> **Context:** Athens is the capital and largest city of Greece. Athens dominates the Attica region and is one of the world's oldest cities, 
             with its recorded history spanning over 3,400 years and its earliest human presence starting somewhere between the 11th and 7th millennium BC.
             Classical Athens was a powerful city-state. It was a center for the arts, learning and philosophy, and the home of Plato's Academy and Aristotle's Lyceum. It is widely referred to as the cradle of Western civilization and the birthplace of democracy, largely because of its cultural and political impact on the European continent—particularly Ancient Rome. In modern times, Athens is a large cosmopolitan metropolis and central to economic, financial, industrial, maritime, political and cultural life in Greece. In 2021, Athens' urban area hosted more than three and a half million people, which is around 35% of the entire population of Greece. Athens is a Beta global city according to the Globalization and World Cities Research Network, and is one of the biggest economic centers in Southeastern Europe. It also has a large financial sector, and its port Piraeus is both the largest passenger port in Europe, and the second largest in the world.

> **Question:** Which is the largest city in Greece?  
  **Prediction:** Athens  
  **True Answer:** Athens  
  **Exact Match:** True  
  **F1 Score:** 1.0

> **Question:** For what was the Athens center?  
  **Prediction:** center for the arts, learning and philosophy  
  **True Answer:** center for the arts, learning and philosophy  
  **Exact Match:** True  
  **F1 Score:** 1.0

> **Question:** Which city was the home of Plato's Academy?  
  **Prediction:** Athens  
  **True Answer:** Athens  
  **Exact Match:** True  
  **F1 Score:** 1.0
