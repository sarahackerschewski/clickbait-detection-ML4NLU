# clickbait-detection-ML4NLU
This is a small script written as part of the ML4NLU course in wintersemester 2022/23 for detecting if a headline is clickbait or not.



The [challenge notebook](https://github.com/sarahackerschewski/clickbait-detection-ML4NLU/blob/main/challenge.ipynb) contains the instructions given. Along with this notebook, we were also given the training data ([clickbait_no](https://github.com/sarahackerschewski/clickbait-detection-ML4NLU/blob/main/clickbait_no) and [clickbait_yes](https://github.com/sarahackerschewski/clickbait-detection-ML4NLU/blob/main/clickbait_yes))

[clickbait_detection_script](https://github.com/sarahackerschewski/clickbait-detection-ML4NLU/blob/main/clickbait_detection_script.ipynb) is the Jupyter Notebook used for the task.
First, the data was split into train and dev. Then, the text was preprocessed (Removal of Punctuation, Lemmatization, TF-IDF). For this classification task, a Naives Bayes (Multibinomial) was chosen and tuned on the dev set. The performance was evaluated with F1-measure (and additionally precision & recall). Finally, the [test set](https://github.com/sarahackerschewski/clickbait-detection-ML4NLU/blob/main/clickbait_hold_X.csv) was given and the classes for this data ([predictions.txt](https://github.com/sarahackerschewski/clickbait-detection-ML4NLU/blob/main/predictions.txt)) was predicted. 

The baseline for this task was an F1 of ~0.89 with a simple classifier. According to the instructors, this NB model achieved an *F1 of 0.969*. The test labels were not made public. 
