Building a spam filter for SMS messages

In this project, the goal was to teach the computer how to classify new messages. 
I used the multinomial Naive Bayes algorithm and a dataset of 5,572 SMS messages already classified by humans. 
The spam filter should have an accuracy greater than 80%.

The dataset was put together by Tiago A. Almeida and Jose Maria Gomez Hidalgo and can be downloaded here:
https://archive.ics.uci.edu/ml/datasets/sms+spam+collection or here:
https://dq-content.s3.amazonaws.com/433/SMSSpamCollection.

For more information about the data collection process check this page:
http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/#composition.

To learn more about the Naive Bayes algorithm, you can check this link:
https://en.wikipedia.org/wiki/Naive_Bayes_classifier

I started by splitting the dataset into 2:
- a training set (about 80% of the data set -  4,458 messages) to use for training our computer on how to classify new messages
- a test set (about 20% - 1,114 messages) to use for testing how good the spam filter is with classifying new messages.

The next step was cleaning the training data set and transforming it into a dataframe.

I then calculcated the constants used in the Naive Bayes algorithm.
I finally built 2 functions:
 - one to classify the messages
 - another one to measure the spam filter's accuracy
 
Conclusion
In this project I managed to build a spam filter for SMS messages using the Naive Bayes algorithm. 
The goal to have at least 80% accuracy was overachieved, we managed to obtain over 98% accuracy.

One of the next steps could be checking the messages that were classified inaccurately and try to improve 
our function. 
