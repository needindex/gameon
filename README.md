# Game On! To Pledge or Not to Pledge? And Why? An Interpretable Prediction Model based on Campaign’s Aspects’ Emotions.

<b>GameOn</b> is a framework to predict the success of Kickstarter campaigns based on the  emotion intensity induced on  domain specific aspects.<br>
The framework enables to automatically mine specific aspects characterizing a domain of interest from a campaign description and products reviews. Our system induces (by means of clustering) a partition of mined domain aspects. The elements of the partition are then used to perform an aspect-based sentiment analysis which combines 8 mood states (i.e. anger, disgust, fear, joy, sadness, interest, admiration and surprise) into a single statistical index, named <i>Need Index</i>. <br>

The <i>Need Index</i> provides the estimated polarities across domain aspects belonging to the same cluster. 
We then build a <i>Need Index</i>-based model to perform predictions on whether the campaign will result into a success, reaching its funding goal.<br> 
Thanks to comprehensible and easy to interpret <i>Need Indexe</i> representation we are able to understand and monitor the most relevant domain aspects trends and the related most predominant perceived mood state.
We experimented our framework on the domain of mobile video games and estimated a competitive prediction accuracy of 94.4% and also compared against domain unaware state-of-the-art systems. 

## Resources
<ul>
  <li> unsupervised induced partition P of domain aspects:<a href="https://github.com/idea2validate/gameon/blob/master/unsupervised_partition.tsv">.tsv</a><br>
    <i>format:</i> cluster_id TAB comma_semparated_list_of_domain_aspects
  </li>
  <li> supervised induced partition P* of domain aspects:<a href="https://github.com/idea2validate/gameon/blob/master/supervised_partition.tsv">.tsv</a><br>
    <i>format:</i> cluster_id TAB cluster_label TAB comma_semparated_list_of_domain_aspects
  </li>
  <li> unsupervised domain-aware (mobile games) dataset P_MG_2009-2019:<a href="https://github.com/idea2validate/gameon/blob/master/dataset_MG_unsupervised_2009_2019.csv">.csv</a><br>
  <i>format:</i> goal,state,c_1,c_2,c_3,c_4,c_5,c_6,c_7,c_8,c_9,c_10,c_11,c_12,c_13,c_14,c_15,c_16,c_17,c_18,c_19,c_20,c_21,	c_22,c_23,c_24,c_25,c_26
  </li>
<li> supervised domain-aware (mobile games)  dataset P*_MG_2009-2019:<a href="https://github.com/idea2validate/gameon/blob/master/dataset_MG_supervised_2009_2019.csv">.csv</a><br>
  <i>format:</i> goal,state,c_1,c_2,c_3,c_4,c_5,c_6,c_7,c_8,c_9,c_10,c_11,c_12,c_13,c_14,c_15,c_16,c_17,c_18,c_19,c_20,c_21,	c_22,c_23,c_24
  </li>
  <li> unsupervised domain-unaware dataset P_DU_2009-2014:<a href="https://github.com/idea2validate/gameon/blob/master/dataset_DU_unsupervised_2009_2014.csv">.csv</a><br>
  <i>format:</i> goal,state,c_1,c_2,c_3,c_4,c_5,c_6,c_7,c_8,c_9,c_10,c_11,c_12,c_13,c_14,c_15,c_16,c_17,c_18,c_19,c_20,c_21,	c_22,c_23,c_24,c_25,c_26,c_27,c_28,c_29,c_30,c_31,c_32,c_33,c_34
  </li>
</ul>


## License
Attribution 4.0 International (CC BY 4.0)

## Contacts
<ul>
<li>Stefano Faralli - University of Rome Unitelma Sapienza, Italy - stefano.faralli at unitelmasapienza.it </li>
<li>Steve Rittinghaus - Independent researcher, Freelancer Digital Transformation, Baden-Württemberg,Germany - steve.rittinghaus at idea2validate.com </li>
<li>Nima Samsami - Independent researcher, Software Architect, Rheinland-Pfalz, Germany,nima.samsami at idea2validate.com </li>
<li>Eugénio Rocha - Center for Research in Mathematics and Applications, Dept. Math., University of Aveiro, Portugal, eugenio at ua.p</li>
<li>Damiano Distante - University of Rome Unitelma Sapienza, Italy - damiano.distante at unitelmasapienza.it</li>
</ul>
