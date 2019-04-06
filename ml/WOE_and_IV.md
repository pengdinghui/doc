##  数据挖掘中的 WOE 与 IV 

WOE的全称是“Weight of Evidence”，即证据权重。WOE是对原始自变量的一种编码形式。

要对一个变量进行WOE编码，需要首先把这个变量进行分组处理（也叫离散化、分箱等等，说的都是一个意思）。分组后，对于第i组，WOE的计算公式如下：


# $WOE_i = ln( \frac{py_i}{pn_i} ) = ln( \frac{ \frac{y_i}{y_t}}{ \frac{n_i}{n_t} } ) = ln( \frac{ \frac{y_i}{n_i}}{ \frac{y_t}{n_t} } )$ 





IV的全称是Information Value，中文意思是信息价值，或者信息量。


# $IV_i = (py_i - pn_i) * WOE_i$


有了一个变量各分组的IV值，我们就可以计算整个变量的IV值，方法很简单，就是把各分组的IV相加：

# $IV = \sum_{i= 1}^n IV_i$

其中，n为变量分组个数。