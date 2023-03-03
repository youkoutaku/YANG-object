![[正規直交基底]]

与えられた[[基底]]から[[正規直交基底]]を構成する方法を**Gram-Schmidtの正規直交化法**という．

[[基底]]：$$\{\mathbf a_1,\mathbf a_2,\dots,\mathbf a_n\}$$

## 直交化
$$b_1=a_2,$$
$$b_2=a_2-\frac {(a_2,b_1)}{(b_1,b_1)}b_1,$$
$$\dots$$
$$b_r=a_r-\frac {(a_r,b_1)}{(b_1,b_1)}b_1-\frac {(a_r,b_2)}{(b_2,b_2)}b_2-\dots-\frac {(a_r,b_{r-1})}{(b_{r-1},b_{r-1})}b_{r-1};
$$

## 正規化
$$c_1=\frac {1}{\|b_1\|}b_1,c_2=\frac {1}{\|b_2\|}b_2\dots,c_r=\frac {1}{\|b_r\|}b_r$$