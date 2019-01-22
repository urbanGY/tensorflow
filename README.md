Tenserflow
==========

> ## 고려할것
> * learning rate를 적절하게. 너무 크면 수렴하지않고(overshooting) 작으면 수렴한다고 착각하게됨
> * 데이터를 zero centered, normalized 하게 바꿔주기
> ** ex) MinMaxScaler(data)로 normalized 가능, 가장큰수를1 작은수를 0으로 하고 비례하게 바꾼다
> * overfiting 방지 위해 regularization 해주기
> ** tensor에서 cost expression + 0.001(constant, regulation strength)*tf.reduce_sum(tf.square(w)) (예시)으로 적용할 수 있다
