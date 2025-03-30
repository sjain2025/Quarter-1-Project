# GPA Genie: Integrating Study Habits, Extracurricular Activities, and Parental Information for GPA Classification

Every year, the stresses placed upon young shoulders become heavier. As time for college applications approach, students lean into cycles of self-doubt and regret, wondering if their in and out of school activities are sufficient to receive an admission letter from the Harvards and Stanfords of the world. Imagine a world where students could control their own destinies. GPA Genie acts as a tool for students to optimize their extracurricular activities from an early age, thereby helping to secure later success. Students will be able to use the tool to weigh different configurations of academic options and decide which ones make the most sense for them. We used the Students Performance Dataset from Kaggle to classify a predicted GPA range given a certain quantitative configuration of study habits, extracurricular, and parental involvement. The class we predicted is called GradeClass, which ascribes the labels 0, 1, 2, 3, 4 to GPAs ranging GPA ≥ 3.5, 3.0 ≤ GPA < 3.5, 2.5 ≤ GPA < 3.0, 2.0 ≤ GPA < 2.5, and GPA < 2, respectively. Our Logistic model trained on the subset AllRetained, where we did not remove any features during preprocessing, produced the highest testing accuracy (75.7322%) of any of the 20 model/subset configurations we tested. As for other metrics permitting to this configuration, we achieved a Precision of 0.869, Recall of 0.757, F1 Score of 0.809, and area under the ROC curve of 0.913. In the future, the accuracy of this model can be improved upon by incorporating additional features like socioeconomic status, school environment, sleep patterns, and more. These factors can provide a more holistic view of a student's environment and habits, which may directly impact their academic performance.

**How to Run:**
1. Navigate to Datasets > AllRetained. Download the files “AllRetained_train.csv” and “AllRetained_test.csv.”
2. Load “AllRetained_train.csv” onto Weka Explorer by clicking “Open file…” under the Preprocess tab.
3. Click “Save…” and save this dataset as “AllRetained_train.arff.”
4. Repeat steps 2 and 3 by loading “AllRetained_test.csv” and saving it as “AllRetained_test.arff.”
5. Open the file “AllRetained_train.arff” by clicking “Open file…” under the Preprocess tab.
6. Navigate to the “Classify” tab and click “Choose.” Then, select the Logistic classifier under classifiers > functions > Logistic.
7. Under “Test options,” select “Supplied test set” and click “Set…”
8. Click “Open file…” in the new pop-up window and select “AllRetained_test.arff.” Then, click “Close.”
9. Click the “Start” button. Weka will display the performance metrics for this model, which achieved an accuracy of 75.7322%.
