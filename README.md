데이터: 호텔리뷰(https://raw.githubusercontent.com/ShivamPatil27/Natural-Language-Processing-on-Restaurent-reviews/refs/heads/master/Restaurant_Reviews.tsv)

데이터 비율: 50:50

모델: Naive Bayes

 CountTokenizer 대신 TF-IDF 사용
 
    ngram_range=(1,2),   # Unigram + Bigram
    
    max_features=5000,   # 상위 5000개 단어만 선택
    
    min_df=2, max_df=0.8, # 너무 흔한 단어/희귀한 단어 제거
    
    sublinear_tf=True,   # 로그 스케일 변환
    
    use_idf=False,       # TF만 사용
    
    norm=None            # 정규화 제거
