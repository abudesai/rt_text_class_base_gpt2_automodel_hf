GPT2 Huggingface Transformer for text (document/sentence) classification, implemented as per Ready Tensor Text Classification - Base specifications.

- text classification
- huggingface
- GPT2
- nlp
- sklearn
- python
- pandas
- numpy
- flask
- nginx
- uvicorn
- docker

This is a Text Classifier that uses a AutoModelForSequenceClassification transformer model implemented through HuggingFace. It uses the GPT2 model and its associated tokenizer.

Data preprocessing step includes HuggingFace's built-in preprocessor for the GPT2 model.

During the model development process, the algorithm was trained and evaluated on a variety of datasets such as clickbait, drug, and movie reviews as well as spam texts and tweets from Twitter.

This Text Classifier is written using Python as its programming language. DistilBert Transformer from HuggingFace is used to implement the main algorithm. SciKitLearn is used for the minor data preprocessing steps such as label encoding and renaming of columns to be what HuggingFace model expects. Flask + Nginx + gunicorn are used to provide web service which includes two endpoints- /ping for health check and /infer for predictions in real time.
