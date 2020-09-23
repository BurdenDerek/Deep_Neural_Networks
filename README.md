# Deep_Neural_Networks
Module 19

How many neurons and layers did you select for your neural network model? Why?

    I went with two layers because the number of features the model was very high and I thought that it would be a good idea to have a second layer to funnel down the number of neurons the output was reading and to filter the input data a tad more.
    The number of neurons for each layer was a little harder to nail down. Without a good intuition for this yet I decided to run trails to find the best one. I made a function to test models with less epochs and save the best of the batch then run a full training seesion on the models that made it past the first stage, then pick best of that bunch.

Were you able to achieve the target model performance? What steps did you take to try and increase model performance?

    I was able to achieve the target model performance 75%. Just finding the best arrangement of neurons in the layers was not enough to reach the target model performance of only 73%. Cleaning and bucketing AAPLICATION_TYPE and CLASSIFICATION was not able to get it all the way there either. It turned out that I mistakenly over looked NAME as an important data point. Unappropriately I assumed that the name of a charity would have no importance on whether they would be a good investment. If our data did not have repeat charities that assumption may have proved to be right; however, that was not the case here and having charities that have already proven themselves to be a good investment means that they are likely to be a safe choice in the future. After including NAME into the analysis and bucketing the charities that we only have a few data points on into a group we were able to raise the target model performance up to 80%.

If you were to implement a different model to solve this classification problem, which would you choose? Why?

    If I had to choose a different model for this problem I was go with the Random Forest. The Random Forest seemed to be able to keep pace with DNN on the examples we did earlier than I was with Logistical Regression.