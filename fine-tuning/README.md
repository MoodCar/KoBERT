# fine-tuning

dataset : https://aihub.or.kr/opendata/keti-data/recognition-laguage/KETI-02-009

7class sentiment analysis

## 모델 세팅

<br/><br/>

### basic

|hyper parameter|value|
|---|---|
|max_len|64|
|batch_size|64|
|epochs|10|
|dropout|0.3(encoder), 0.5(cls)|
|label_smoothing|0.0|
|lr|2.5e-5|

<br/>

train accuracy : 63.55


test accruacy : 55.08

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

### Layer-wise Decreasing Layer Rate

|hyper parameter|value|
|---|---|
|max_len|64|
|batch_size|64|
|epochs|10|
|dropout|0.1|
|epsilon|0.95|
|lr|2.5e-5|
|label smoothing|0.3|

<br/>
test accuracy : 53.8


### Layer-wise Decreasing Layer Rate drop 놀람 data

|hyper parameter|value|
|---|---|
|max_len|64|
|batch_size|64|
|epochs|10|
|dropout|0.1|
|label smoothing|0.0|
|epsilon|0.95|
|lr|2.5e-5|

<br/>
test accuracy : 57.45


<br/>
<br/>
<br/>
참고논문:

[How to Fine-Tune BERT for Text Classification?(ITPT)](https://arxiv.org/abs/1905.05583)
