# topic-modelling-indonesian-health-influencer-tweet

This repository consists of topic modelling with Latent Dirichlet Allocation (LDA) algorithm for indonesian health influencer tweet. The exploration also include visualization of Wordcloud to show the frequently occuring words of all the tweet and for each influencer.

# Dataset
The dataset is extracted and collected from Twitter with Twitter API and tweepy library from 7 health influencer in Indonesia in Januari and February 2022. The dataset is consists of indonesian, english,  and mix of those two languages.

# Result
## Wordcloud
Overall, the discussion on the dominant health influencer account tweets about matters surrounding COVID-19 which are represented by the words vaccines, medicines, and homes. In addition, many tweets also convey health messages such as paying attention to diet, sleeping hours, sleep, thoughts, and symptoms. 
From the words that often appear in all data and for each account, it can be concluded that the most common discussion in health sector tweets is about COVID-19.
However, if you take a deeper look at each account, each influencer account has its own dominant discussion. Two influencer accounts like jiemiardian and
asaibrahim were found to have discussions that emphasized health education regarding their respective professional fields.

## LDA Model Experiment
The LDA model shows that each number of topic has it's best alpha and beta numbers. The experiment is measured by three metrics as stated below
1. Coherence: shows that the best model is model with n_topics 3 with alpha = 0.31 dan beta = 0.11, the score is 0.538
2. Perplexity: shows that the best model is model with n_topics 5 with alpha = 0.61 dan beta = 0.41., the score is -6.196
3. Percent contribution score of word in each sentences: in the top ten and one hundred sentences that have the largest percent contribution of each topic, the results of tuning the model number of topics = 3 have the largest average. In the top ten sentences, the percent contribution scores 95.2% and in the top one hundred sentences it reached 89.8%. This shows that the number of topics = 3, a lot of words in the sentences that match the words that appear in the results of the topic modeling.

It's conclude that the best model is model with n_topic = 3 in this datase. With overall topics are stated below.
1. Topic 1
- indonesian : pikir, doa, emosi, teman, hidup, positif, hati, ulang, foto, chenle
- english : thoughts, prayers, emotions, friends, life, positive, heart, birthday, photos, chenle
2. Topic 2
- indonesian : tidur, makan, covid, rumah, jam, pagi, malam, minum, selamat, anak
- english : sleep, eat, covid, home, hours, morning, night, drink, safe, child
3. Topic 3
- indonesian: vaksin, covid, obat, bpjs, paham, gejala, layan, anak, booster, ganggu
- english : vaccine, covid, medicine, bpjs, understand, symptoms, service, child, booster, disturb

Align with Wordcloud result, majority of topic is about COVID-19 with some variations related to the main topic in each health influencer that has difference profession.


