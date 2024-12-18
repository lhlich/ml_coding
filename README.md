# ML coding
In this repo I'd build a few examples to show how various ML algorithms works.

### Classical Machine learning
Relevant algorithms:
- ✅Linear regression/logistic regression
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/linear_regression.ipynb)
  - [Another notebook with illustration on gradient descent](https://github.com/lhlich/ml_coding/blob/master/classic_ml/linear_regression_gradient_descent.ipynb)
- ✅kNN classfication/regression 
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/kNN.ipynb)
- ✅k-means clustering
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/kMeans.ipynb)
- ✅Naive Bayes
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/naive_bayes.ipynb)
- ✅Cross Valdiation
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/cross_validation.ipynb)
- ✅PCA
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/PCA.ipynb)
- ✅AUC metric
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/AUC.ipynb)
- Boosting/xgboost
  
### Deep learning
Neural network general:
- Autograd
- ✅optimizers: SGD, Adam, RMSProp
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/deep_learning/optimizers.ipynb)
- ✅Gradient computation
- Backpropagation
- Integrated gradient feature importance
- Tensorboard usage
  
Recsys:
- ✅Collaborative filtering
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/classic_ml/colaborative_filtering.ipynb)
- Pytorch lightening
- TorchRec
  
NLP related:
- ✅TF-IDF
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/nlp/tf_idf.ipynb)
- ✅CharRNN
  - [blog post](https://karpathy.github.io/2015/05/21/rnn-effectiveness/), [Karpathy's repo](https://github.com/karpathy/char-rnn?tab=readme-ov-file)
  - The goal is to redo the charRNN example in the book "hands on machine learning". There already provided an [example using tf and keras](https://github.com/ageron/handson-ml3/blob/main/16_nlp_with_rnns_and_attention.ipynb)
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/nlp/charrnn.ipynb)
- Transformer from scratch
- PyText
- ✅[Contrastive decoding](https://arxiv.org/abs/2210.15097) with Hugging
    - [Notebook](https://github.com/lhlich/ml_coding/blob/master/nlp/contrastive_decoding.ipynb)
- RAG. [guide](https://www.youtube.com/watch?v=wd7TZ4w1mSw&list=PLfaIDFEXuae2LXbO1_PKyVJiQ23ZztA0x) from LangChain
  - ✅Basic RAG
    - [Notebook](https://github.com/lhlich/ml_coding/blob/master/nlp/RAG.ipynb)
  - Raptor

ML infra:
- Iterator for nested array.
- In memory SQL engine
- Spreadsheet with math equation

Reinforcement learning
- Use [openAI Gym library](https://github.com/openai/gym) to setup games
- PPO for CartPole 
- DQN for CartPole

Statistics:
- ✅random sample with weights
  - There is a die with $n$ sides. The probability of each side of the die is $p_i$. Write a function to generate $m$ rolls from such die.
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/statistics/random_sample.ipynb)
- ✅design rand10() using rand7
  - [Notebook](https://github.com/lhlich/ml_coding/blob/master/statistics/rejection_sampling.ipynb)