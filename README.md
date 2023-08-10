# Sentiment-Analysis-CHN-ML-LSTM-BERT-TextCNN
This repository records my learning of Chinese sentiment analysis in natural language processing courses, including the use of machine learning and deep learning methods, including LSTM, BERT, TextCNN and other models.

## 1. Dataset: 

### ChnSentiCorp_htl_all(see at data)
### e.g. 

|label|text_a|
|:----:|:----:|
|1 |	选择珠江花园的原因就是方便，有电动扶梯直接到达海边，周围餐馆、食廊、商场、超市、摊位一应俱全。酒店装修一般，但还算整洁。 泳池在大堂的屋顶，因此很小，不过女儿倒是喜欢。 包的早餐是西式的，还算丰富。 服务吗，一般|
|1 |	15.4寸笔记本的键盘确实爽，基本跟台式机差不多了，蛮喜欢数字小键盘，输数字特方便，样子也很美观，做工也相当不错|
|0 |	房间太小。其他的都一般。。。。。。。。。|

## 2. Notebook:
every note book contain a method to solve the problem(except the "ml.ipynb").
every method provide single-predict and muti-predict function

## 3. result
### ML method

PS: use tf-idf to extract feature 

|method|accuracy|precision|recall|f1-score|
|:----:|:----:|:----:|:----:|:----:|
|svm	|0.8975	|0.8975	|0.8975	|0.8975|
|lr	|0.8875	|0.8875	|0.8875	|0.8875|
|nb	|0.8792	|0.8792	|0.8791	|0.8791|
|rf	|0.8992	|0.8999	|0.8995	|0.8992|
|dt	|0.8083	|0.8087	|0.8086	|0.8083|
|ada	|0.7850	|0.7855	|0.7853	|0.7850|
|gb	|0.8175	|0.8234	|0.8184	|0.8169|
|sgd	|0.8992	|0.8992	|0.8992	|0.8992|
|bag	|0.8300	|0.8356	|0.8309	|0.8295|

### DL method
|method|accuracy|
|:----:|:----:|
|LSTM |0.6300|
|BiLSTM| 0.8633|
|TextCNN| 0.9175|
|BERT |0.9542 |

## 4. train:
Except for the Bert model, all other models can be trained in a short period of time on RTX2060, and the notebook contains methods for saving and loading the optimal model.
