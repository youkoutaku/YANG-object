# 1.Python入門
## 1.3.1　算術計算
乗算：
```python
2*2
```

除算：
```python
2/2
```

累乗：
```python
2*2
```

## 1.3.2　データ型(data type)
データ型を確認する関数：
```python
type()
```

データ型：
-  整数型(int)
-  浮動小数点型(float)
-  文字列型(str)

## 1.3.3　変数(variable)
定義
	
## 1.3.4　リスト(list)
リスト作成：
```python
a=[1,2,3,4,5]
```

リストの長さ：

```python
len(a)
```


要素アクセス：
```python	
a[0],a[1]…
```

値の代入：

```python	
a[4]=9
```

サブリストへアクセス：

```python
a[0:2]  #0番目から2番目(2番目が含まない）まで取得
a[1:]  	#1番目から最後まで取得
a[:3]  	#最初から3番目（3番目が含まない）まで取得
a[−1:]  #最後の要素のひとつ前まで取得
a[:−1]	#最初から最後の要素のひとつ前まで取得
```

## 1.3.5　ディクショナリ(dictionary,辞書)
キーと値をペアとしてデータを格納する

```python	
	me={'height':180}
    me['height']
    180
	me['weight']=70
    print(me)
	{ 'height':180, 'weight':70 }
```

## 1.3.6　ブーリアン(boolean)
bool型(True or False)
論理演算子

```python	
    not 
	and
	or
```

## 1.3.7　if文
条件に応じて，処理を分岐する
```python	
if a<0 :
	print()   
else:
	print()
```

インデントを表すために，4つの空白文字を使う    
	
## 1.3.8　for文
ループ処理

```python	
for i in [1,2,3]:
	print(a)
```
## 1.3.9　関数(function)
関数を定義する

```python	
def hello():
	print("Hello World!")	
```

## 1.4.2　クラス(class)
ユーザーが自分でクラスを定義する．

```python	
class クラス名：
	def __init__(self,引数, …):  #コンストラクタ(constructor,構造関数)
	…
	def メソッド名(self,引数, …): #メソッド1(method,方法)
	…
def メソッド名(self,引数, …): #メソッド2
	…
```
__intit__と言う特別なメソッドは，クラスのインスタンス(instance)が作成されるための初期化用のメソッドである．
例として:

## 1.5　NumPy
インポート

```python	
import numpy as np
```


## 1.5.2　NumPy配列の生成
Pythonのリストを引数に取り，NumPy用の配列(numpy.ndarray)を作成する．

```python	
x = np.array( [1.0, 2.0, 3.0] )
```

## 1.5.3　NumPyの算術計算
NumPy配列の計算：
配列の要素数が同じ場合，算術計算は各要素に対して行われる．
要素数が違う場合，「エラー」になる．
「要素ごと」：element-wise

```python	
    import numpy as np
    x = np.array( [1.0, 2.0, 3.0] )
    y = np.array( [2.0, 4.0, 6.0] )

    x+y
    array([3., 6., 9.])
    x-y
    array([-1., -2., -3.])
    x/y
    array([0.5, 0.5, 0.5])
    x*y
    array([ 2.,  8., 18.])
    
```

NumPy配列とスカラー値の組み合わせて算術計算を行う．
```python	
    x = np.array( [1.0, 2.0, 3.0] )
    x /2.0
    array([0.5, 1. , 1.5])
```

## 1.5.4　NumPyのN次元配列

```python	
    A = np.array( [[1, 2], [2, 3]] )
    print(A)
    [[1 2]
    [2 3]]
	
    A.shape #行列の形状
    (2, 2)

    A.dtype #要素のデータ型
    dtype('int32')

    B = np.array( [[3, 0], [0, 6]] )
    A+B
    array([[4, 2],
       [2, 9]])
    
    A*B
    array([[ 3,  0],
       [ 0, 18]])

    A*10
    array([[10, 20],
       [20, 30]])
```

## 1.5.5　プロードキャスト
