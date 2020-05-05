# Sentiment-Classification-Using-ULMFiT-and-Tranfer-learning

* This is a sentiment classification project using [FastAi](https://github.com/fastai/fastai) deep learning library.
* The goal is to classify cell phones reviews as positive and negative.
* The dataset is made by web scraping n11.com website for mobile phones comments. The data consists of 6597 pozitive and 1284 negative comments.
* ULMFit is used as the architecture for the deep learning model. 
* Turkish Wikipedia (vikipedia)  is used for the building of the languaage model.([link](https://dumps.wikimedia.org))
* I used the [WikiExtractor](https://github.com/attardi/wikiextractor) script to clean the wikipedia data.
* Transfer Learning (from the language model) is used for trining.

I was able to gain a 88% accuracy on the validation set. the accuracy on an unseen test set is not yet tested.

The 88% is propably **not** very accurate for the following reasons: 

1. The data is contained of nearly 6000 positive and a 1000 negative comments. To balance this inequality and help the model to learn the negative comments I aggregated the negative comments to get 2000 negative comment. 
2. Due to the low number of negative comments. The negative data is not a good example of a general negative comment. 
3. When I inspected the data I noticed a lot of pozitive comments labeled as negative and vice versa. 

## Further To do's:
* Test the model on an unseen test set
* Collect more data (especially negative comments).
* Clean the data of wrong labels

* Fix the data (some turkish letters are written as english ones, 'u' instead of 'ü', 'i' instead of 'ı' and so on)


