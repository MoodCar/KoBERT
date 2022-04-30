# fine-tuning

## 모델 세팅

<br/><br/>

### basic



<br/>

### ITPT

|hyper parameter|value|
|---|---|
|max_len|64|
|batch_size|64|
|epochs|10|
|dropout|0.1|
|epsilon|0.95|
|lr|2.5e-5|


<br/>
test accuracy : 54.8

### ITPT with label smoothing

|hyper parameter|value|
|---|---|
|max_len|64|
|batch_size|64|
|epochs|10|
|dropout|0.1|
|epsilon|0.95|
|lr|2.5e-5|
|smoothing|0.3|

<br/>
test accuracy : 53.8


### ITPT drop 놀람 data

|hyper parameter|value|
|---|---|
|max_len|64|
|batch_size|64|
|epochs|10|
|dropout|0.1|
|epsilon|0.95|
|lr|2.5e-5|

<br/>
test accuracy : 57.45


<br/>
<br/>
<br/>
참고논문:

[How to Fine-Tune BERT for Text Classification?(ITPT)](https://arxiv.org/abs/1905.05583)
