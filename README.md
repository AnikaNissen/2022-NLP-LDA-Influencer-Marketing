# Research Project:
# Social Media Marketing // Influencer Marketing


##  Research Goal:
 Get an overview of the different topics that are investigated in related literature,
 and then see in how far virtual/GCI/AI influencers are already investigated in literature as part of the overall corpus



### Procedure — Data Collection:
 Conduct a Structured Literature Review on Scopus to receive a list of literature

 Search Date: October 26th 2022

 Search String:
 TITLE-ABS-KEY((influencer AND "social media")) AND ( LIMIT-TO ( LANGUAGE,"English" ) )

 Results:
 1,882 document results

 => Results are exported to CSV from Scopus: ``SociaMediaInfluencer-ScopusData.csv``


### Procedure — Data Synthesis & Analysis:
These steps are done in the jupyter notebook: ``Influencer Marketing Literature - LDA Analysis.ipynb``
<br>
* CSV-File is read into the jupyter-notebook
* text from the abstracts is tokenized, stemmed, and lemmatized using the NLP SpaCy library
* Latent Dirichlet Allocation (LDA) is run to cluster the tokenized text data into different topic clusters
* LDA model for 1 < N < 30 topics is calculated to get the best number of topics in terms of coherence
* Number of Topics with best coherence score is calculated, translated back into the data sheet and visualized using pyLDAvis


### To run the notebok prior explained use the following prompt:
* Use the file ``req.txt`` to install all necessary packages with ``conda create -n <environment-name> --file req.txt``
* Also make sure you have the SpaCy language model installed for the normal analysis: ``python -m spacy download en_core_web_sm``
* If you want to use the more precise languag model then: ``python -m spacy download en_core_web_trf`` and run the notebook with the ``TRFModel`` attachment


### Results:
#### Main Takeaways:
We seem to have overall about 7 major topics that can be grouped into the following subjects:
* Influencers that post their opinions on twitter, and people searching for opinions on twitter
* There seemed to be a special trend to turn to social media for help in times of the COVID pandemic
* Brand marketing and seeking infos about brands through influencers
* The brand seeking behavior - especially for fashion - is often associated with Instagram
* The research stream on Twitter influencers seems to be different from the Facebook/Youtube/Instagram research

#### Resulting Topics and Number of Papers associated with topic:
* Topic 1: N = 941 Papers have the topic "0.018x"influencer" + 0.012x"face" + 0.012x"argue" + 0.012x"change" + 0.010x"need" + 0.010x"examine" + 0.009x"woman" + 0.008x"draw" + 0.008x"focus" + 0.008x"use""
* Topic 2: N = 406 Papers have the topic "0.017x"identify" + 0.014x"influencer" + 0.012x"understand" + 0.012x"provide" + 0.011x"share" + 0.011x"pandemic" + 0.011x"explore" + 0.011x"include" + 0.010x"relate" + 0.010x"help""
* Topic 3: N = 340 Papers have the topic "0.059x"influencer" + 0.032x"brand" + 0.028x"consumer" + 0.013x"provide" + 0.013x"smi" + 0.013x"follower" + 0.012x"product" + 0.011x"affect" + 0.010x"marketer" + 0.010x"create""
* Topic 4: N = 101 Papers have the topic "0.044x"instagram" + 0.013x"facebook" + 0.013x"examine" + 0.012x"provide" + 0.011x"engage" + 0.010x"influencer" + 0.010x"content" + 0.010x"youtube" + 0.009x"share" + 0.009x"include""
* Topic 5: N = 60 Papers have the topic "0.025x"twitter" + 0.023x"result" + 0.020x"tweet" + 0.018x"conclusion" + 0.018x"include" + 0.014x"increase" + 0.014x"method" + 0.013x"analyze" + 0.012x"post" + 0.012x"compare""
* Topic 6: N = 25 Papers have the topic "0.030x"identify" + 0.022x"user" + 0.020x"twitter" + 0.020x"influencer" + 0.019x"base" + 0.014x"information" + 0.014x"find" + 0.014x"influence" + 0.014x"propose" + 0.011x"spread""
* Topic 7: N = 9 Papers have the topic "0.023x"influence" + 0.021x"finding" + 0.021x"examine" + 0.019x"affect" + 0.016x"intention" + 0.014x"investigate" + 0.014x"purpose" + 0.014x"purchase" + 0.013x"value" + 0.012x"originality""
