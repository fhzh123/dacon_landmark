dacon link: https://dacon.io/competitions/official/235658/overview/

## 12월 7일 02:00
아이디어:
- sklearn, 등을 통해 단어 빈도 기반의 모델 생성 필요
- 일정 confidence 이하 문장에 대해서 단어 빈도 기반 모델 접목
변경점:
- 단어 빈도 기반의 모델 -> 약 93-94%대의 성능

## 12월 8일 01:30
아이디어:
- 일정 confidence 이하 문장에 대해서 단어 빈도 기반 머신러닝 모델 접목
- RNN에 src_total 투입 / 성능 비교 필요
변경점:

## 12월 8일 15:00
아이디어:
- Knowledge distillation 필요

## 12월 9일 15:00
아이디어:
- Khaiii, mecab, 등 KoNLPy도입
- Embedding에 noise추가

## 12월 10일 02:00
아이디어:
- Embedding에 noise추가
변경점:
- KoNLPy, Khaiii 추가
- 현재 수정중 (아직 안돌아감, 각 parser마다 인풋의 크기가 달라서 concat이 안됨)

## 12월 12일 02:00
아이디어:
- 일부 토큰만 사용하는 것이 아닌 전체 토큰에 pooling 진행
- LSTM도 진행
- Word2Vec 학습
변경점:
- 이전에 수정한 KoNLPy, Khaiii에 대해서 학습 가능

## 12월 13일 03:00
아이디어:
- max pooling시 activation function 도입
변경점:
- 일부 토큰만 사용하지 않고 전체 토큰에 대해서 max pooling 진행

## 12월 13일 13:00
아이디어:
- K-Fold validation, 등을 통해 train데이터에서 자꾸 틀리는 것만 모아두기

## 12월 14일 16:00
아이디어:
- Conditional BERT로 Augmentation 진행
- 데이터 불균형 해소 필요
변경점:
- Khaiii가 제대로 parsing되지 않던거 수정
- Print쪽 오류 수정

## 12월 20일 03:00
아이디어:
- 정말 큰 모델을 만들어 보자
- Total과 content 모두 넣어서 싸그리 학습
- LSTM, SRU, 등 그냥 있는대로 다 때려박고 진행해보자

## 12월 22일 01:00
아이디어:
- 다 떄려박는 모델 만들기는 하는데, 어떤 식으로 합칠지 고민
- 논문(https://openreview.net/pdf?id=rylnK6VtDH) 참조도 고려
변경점:
- LSTM 추가
- Total, Content only 버젼 추가만 되어있음, 코드 수정 필요