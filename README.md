# ABSA

The SOTA paper and code referred for the task is : 
Utilizing BERT for Aspect-Based Sentiment Analysis via Constructing Auxiliary Sentence (2019) by Chi Sun, Luyao Huang and Xipeng Qiu

Link to paper : https://arxiv.org/abs/1903.09588

# Description
Utilized a BERT model for the task of Aspect Based Sentiment Analysis. Referred approach and code from the SOTA paper referred above and made appropriate changes:
Please refer to the prepareJsonLines function in evaluation.py file for inspecting the following changes :
1. Extracted trueLabels and predictedLabels(along with scores) from results.
2. Created JSONs with appropriate keys and values (as per the requirements), and appended to a JSONLines file.
3. Maintained counts of correctly labelled instances in terms of aspects and their respective sentiments.
4. Maintained counts of incorrectly labelled instances in terms of aspects.
5. Compared the numbers for evaluating the model's performance on different aspects.

# Suggested optimizations/improvements :
1. Try evaluating the model multiple times during an epoch.
2. Try identifying bad initializations early and stopping them.
3. Try training BERT with the same hyperparameters as in the original setup, but with different random seeds.
4. Try other sophisticated model architectures like ALBERT, RoBERTa, DistilBERT, XLNet after literature survey.
