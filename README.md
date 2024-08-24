# deep-learning-challenge
Module 21
Open Google Colab (through a Google search).
Import/upload the starter code from the HW assignment.
Complete the preprocessing, compiling, training, and evaluation based on the comments.
Save/export original file.

On second and third attempt, repeat the above process, but edit the training section to attempt to improve the model.

Final analysis is available in the "Analysis.docx" file.


Analysis
1. The goal of this project was to use a neural network to test the success rate of organizations that received money from the Alphabet Charity.  By training past recipients, hopefully in the future Alphabet Charity recognizes applicants who will be successful with donations from our charity.
2. Data Preprocessing
•	First, remove unnecessary columns such as name and EIN.
•	The “Is_Successful” column is important because our end goal is to donate money to successful organizations, and this is the column we track past success stories.  We are looking for the 1 in the column as that means true rather than 0 which equates to false/unsuccessful.  Under- and overfitting is a concern when I see the difference between the training and testing numbers.
•	Other possible important features could be “Organization” or “Income_Amt,” though they weren’t factored during this test.

Compiling to Evaluating
•	I was conscientious of the total parameters, but I started with the example given of two hidden layers, one with 80 and one with 30 neurons.  Both had relu activation and the one output layer had a sigmoid activation feature.  I used 100 epochs as that seemed to be the most common from past examples and wouldn’t strain the system too much.  
•	I did not achieve over 75% in the model.  On the second attempt, I increased the number of neurons to 100 and 45 respectively and changed the activation to sigmoid in the hidden layers.  Then, on the third attempt, I added a third hidden layer.   Though the accuracy improved over the three attempts, it did not get above 75%.
4. Overall, my model improved slightly with some adjustments and it could predict a successful donation with 74% accuracy.  I could change the binning options or continue to adjust at the “define the model” stage to get more accuracy in the future.  Though 75% is okay when predicting donation distribution, an improvement would be more fiscally sound moving forward and I would try other options.  
