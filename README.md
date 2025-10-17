# Analysis-of-Health-on-Various-Continents---LLM-Project
LLM -> Experiments -> Final testing  

Cleaned data

Pre-Processing Data

Train 80% post train dataset to LLM paraphrase is humarin/chatgpt_paraphraser_on_T5_base 

I trained the paraphrased batch per batch. All three will be combined.

80%Post train dataset + 80% Post Paraphrased.

We will proceed to Experiment:

Experiment# 1 : 80% post train dataset and validation set 

Experiment# 2 : 80% post train dataset + 20% Paraphrased and validation set

Experiment# 3 : 80% post train dataset + 50% Paraphrased and validation set

Experiment# 4 : 80% post train dataset + 100% Paraphrased and validation set

Experiment# 5 : 100% post train dataset + 100% Paraphrased and validation set

All models will be trained each of experiment will be distributed to each model.
"Logistic Regression", "Naive Bayes", "SVM (LinearSVC)", "Random Forest", "XGBoost"


Results of the model:
Final F1 (macro) table (Model x Experiment):

Experiment                1       2       3       4       5

Model

Logistic Regression  0.7666  0.7755  0.7812  0.7939  0.8667

Naive Bayes          0.7353  0.7424  0.7398  0.7429  0.7945

Random Forest        0.7392  0.7465  0.7576  0.7616  0.9993

SVM (LinearSVC)      0.7505  0.7599  0.7697  0.7880  0.9251

XGBoost              0.7589  0.7585  0.7687  0.7756  0.9056

Final Testing will be 

Experiment 3 -> Test dataset -> result

Final Results:

                 Model  Accuracy  F1_macro
                 
  Logistic Regression  0.671141  0.667880

          Naive Bayes  0.627517  0.631163

      SVM (LinearSVC)  0.674497  0.670725

         Random Forest  0.644295  0.644478

              XGBoost  0.590604  0.585720
