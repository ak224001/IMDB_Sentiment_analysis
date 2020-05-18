# Sentiment-analysis
classification of emotions (positive, negative) within text data.
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/text.png" width="350" title="Nlp_img">
</p>
<h2> Dataset</h2>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/img/df_head.png"  title="df_head">
</p>
<h2>Average length of text</h2>
<p>
Average length of review in training dataset 122.12678</br>
Std Deviation  of review in training dataset 92.0244301630366
<p>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/AvgLen.png"  title="Avg_length">
</p>
<h2>Architechture</h2>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/architechture.png"  title="Arch">
</p>
<h2> Build Model</h2>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/model_arch.png"  title="Build_Model">
</p>
<h2>Train Model</h2>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/model_acc.png" title="Model_train">
</p>
<h2>Model Accurancy</h2>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/modelAccuracy.png"  title="Build_Model">
</p>
<h2>Model loss</h2>
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/master/Images/modelLoss.png" title="Model_train">
</p>
<h2>Test model</h2>
We can test our model with some sample reviews to check how it is predicting the sentiment of each review. First we will have to convert the text review to tokens and use model to predict as below.
<p align="center">
  <img src="https://github.com/ak224001/IMDB_Sentiment_analysis/blob/img/Test.png" title="Model_train">
</p>
<h2>Test model on some real sample</h2>

<b>com1</b>= "To be honest, this is the movie that motivated me to read the book of Exodus. I watch this movie again and again and it has blessed me so much. Exodus contains many precious truths about our blessed Lord Jesus Christ. It contains pictures, types, and the applications (like the blood on the doorpost) which have direct meaning on our Christian life today. Please do watch this movie and be blessed. See how the LORD planned beforehand and chose a deliverer to free the children of Israel and give them freedom, performed mighty miracles through him to save the children of Israel from the bitter bondage, protected Israel from the Pharaoh and his soldiers who sought to kill and destroy them, see the LORD's glory and His ways. Praise be to His wonderful name!"

<b>com2 </b>= "Highly impressed with the movie and it is an inspreration of my faith too be more stronger . I love this movie to watch again and again to be one off  the best believer . Thank you soo very much for the making of this movie. Love you and God bless the entire team .Blessings to all of you , who is sharing this for free ."

<b>com3 </b>= "I have always loved this movie. It is the best depiction of the bible on screen that I have watched. Also, Cecil B. DeMille was Jewish, so he wanted to get as close to the Bible as possible in making this movie. One of Charlton Heston's and Yul Brynner's best pictures...they were fantastic!!!"

<b>com4 </b>= "The greatest epic director was DeMille. However he cast that wooden actor for his looks and not for his acting skill , Charles Heston as Moses. Read all about DeMille in THE LOST  WORLD of DEMILLE by   JOHN KOBAL  DeMille cast his main characters in his epic biblical movies based on European art work who painted the great Jewish characters as tall virile Christians with long flowing hair. He forgot to consult his mother Jewish side for how people looked "

<b>com5 </b>= "I watched this movie around 20 years ago almost every friday night mainly because  i enjoyed it so much. Now that im alot older and understand it more i enjoy it alot more. Im not religious now but it really gives you a good understanding of the story of Moses."

<b>com6 </b>= "The movie was, is and will be amazing forever. All the actors had done a very good job. Excellent photography, costumes, biggest movie all the time with the imperishable Word of God from Exodus. All glory, paise, and honor to Almighty God,Who created Heaven and earth."

<b>com7 </b>= "For 1956 it was great. I was only 9, buI like to see it in 2019. The God I serve did part the Red Sea to save His chosen people. The very same God sent his only son to die so that we can have eternal life. Tomorrow I celebrate Easter because Jesus rose from the grave and one day soon He is coming back to claim His own. He is pure love."

<b>com8 </b>= "This movie delivers the respect an adaptation of the life of Moses deserves. It truly is one of the greatest films of all time. I once wrote a review for 'Prince of Egypt' which I thought was better but it depends on what you want to see. if you want to see a good character study of Moses, watch this movie. If you just want to watch an action movie or a musical or a kids movie, watch that one."

<b>com9 </b>= "This movie was AMAZING!!!! I'm an atheist and I loved it a lot!! honestly i don't know who Moses is but he seemed like a real jerk in my opinion, but everyone else in the movie seemed fine to me. 8/10 would recommend to my atheist Facebook group."

<b>com10 </b>= "Wonderful film about the children of Israel as they are in bondage in Egypt. They experience and see the hand of God through the 10 plagues. Finally  the Lord rescues them then guides them through the wilderness and calls them to be His people and covenants to be their God. Its an epic film showing the importance of obedience and faith in God the Father of Abraham, Isaac and Jacob."
comments = [com1,com2,com3,com4,com5,com6,com7,com8,com9,com10]
<h3>
 First we will have to convert the text review to tokens and use model to predict.</h3>
  
## model.predict(com_token_pad)
array([[0.9442054 ],</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [0.9882251 ],</br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      [0.93999845],</br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      [0.88237476],</br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;     [0.97660553],</br>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  [0.9667096 ],</br>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   [0.8522855 ],</br>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  [0.9893428 ],</br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  [0.7957951 ],</br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[0.9764207 ]], dtype=float32)</b>

## Thank you
