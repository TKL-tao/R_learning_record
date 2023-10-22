---
title: "Untitled"
output: github_document
---








# Q1
## (a)
### For attribute class,
$Info(class)=1-(\frac{7}{16})^2-(\frac{9}{16})^2=0.4922$

### For attribute A
#### $\theta_a=2:$

$P(A<2)=\frac{2}{16}$

$P(A>2)=\frac{14}{16}$

$Info(class_{A<\theta_a})=1-1^2-0^2=0$

$Info(class_{A>\theta_a})=1-(\frac{5}{14})^2-(\frac{9}{14})^2=0.4592$

$Gain(class, A)=Info(class)-Info_A(class)=0.4922-\frac{2}{16}\cdot0-\frac{14}{16}\cdot0.4592=\color{red}{0.0904}$

#### $\theta_a=5:$


$P(A<5)=\frac{8}{16}$

$P(A>5)=\frac{8}{16}$

$Info(class_{<\theta_a})=1-(\frac{3}{8})^2-(\frac{5}{8})^2=0.4688$

$Info(class_{>\theta_a})=1-(\frac{4}{8})^2-(\frac{4}{8})^2=0.5$

$Gain(class, A)=Info(class)-Info_A(class)=0.4922-\frac{8}{16}\cdot0.4688-\frac{8}{16}\cdot0.5=\color{red}{0.008}$

#### $\theta_a=8:$


$P(A<8)=\frac{13}{16}$

$P(A>8)=\frac{3}{16}$

$Info(class_{<\theta_a})=1-(\frac{6}{13})^2-(\frac{7}{13})^2=0.4970$

$Info(class_{>\theta_a})=1-(\frac{1}{3})^2-(\frac{2}{3})^2=0.4444$

$Gain(class, A)=Info(class)-Info_A(class)=0.4922-\frac{13}{16}\cdot0.4970-\frac{3}{16}\cdot0.4444=\color{red}{0.0051}$

<font size='5'>The threshold 2 of A provides the largest reduction in impurity of node class. Therefore, $\theta_a=2$.</font>

## (b)
### For attribute B


$P(B='yes')=\frac{8}{16}$

$P(B='no')=\frac{8}{16}$

$Info(class_{B=yes})=1-(\frac{4}{8})^2-(\frac{4}{8})^2=0.5$

$Info(class_{B=no})=1-(\frac{3}{8})^2-(\frac{5}{8})^2=0.4688$

$Gain(class, B)=Info(class)-Info_B(class)=0.4922-\frac{8}{16}\cdot0.5-\frac{8}{16}\cdot0.4688=\color{red}{0.0078}$

### For attribute C


$P(C='yes')=\frac{9}{16}$

$P(C='no')=\frac{7}{16}$

$Info(class_{C=yes})=1-(\frac{3}{9})^2-(\frac{6}{9})^2=0.4444$

$Info(class_{C=no})=1-(\frac{4}{7})^2-(\frac{3}{7})^2=0.4898$

$Gain(class, C)=Info(class)-Info_C(class)=0.4922-\frac{9}{16}\cdot0.4444-\frac{7}{16}\cdot0.4898=\color{red}{0.0279}$

<font size='5'>Attribute A with $\theta_a=2$ should firstly be used for developing a decision tree.</font>

# Q2
## (a)
### For attribute d2,

$Info(d2)=1-(\frac{10}{20})^2-(\frac{10}{20})^2=0.5$

### For attribute a3,


$P(a3='yes')=\frac{13}{20}$

$P(a3='no')=\frac{7}{20}$

$Info(d2_{a3='yes'})=1-(\frac{4}{13})^2-(\frac{9}{13})^2=0.4260$

$Info(d2_{a3='no'})=1-(\frac{6}{7})^2-(\frac{1}{7})^2=0.2449$

$Gain(class, d2)=Info(d2)-Info_{a3}(d2)=0.5-\frac{13}{20}\cdot0.4260-\frac{7}{20}\cdot0.2449=\color{red}{0.1374}$

### For attribute a5,


$P(a5='yes')=\frac{4}{20}$

$P(a5='no')=\frac{16}{20}$

$Info(d2_{a5='yes'})=1-(\frac{3}{4})^2-(\frac{1}{4})^2=0.3750$

$Info(d2_{a5='no'})=1-(\frac{7}{16})^2-(\frac{9}{16})^2=0.4922$

$Gain(class, d2)=Info(d2)-Info_{a5}(d2)=0.5-\frac{4}{20}\cdot0.3750-\frac{16}{20}\cdot0.4922=\color{red}{0.0312}$

<font size='5'>Attribute a3 should firstly be used for developing a decision tree.</font>

## (b)
$P(d2=yes)=\frac{10}{20}$

$P(d2=no)=\frac{10}{20}$

$P(a1=40.0|d2=yes)=P(a1>\theta_1|d2=yes)=\frac{9}{10}$

$P(a2=yes|d2=yes)=\frac{0}{10}$

$P(a3=no|d2=yes)=\frac{1}{10}$

$P(a1=40.0|d2=no)=P(a1>\theta_1|d2=no)=\frac{0}{10}$

$P(a2=yes|d2=no)=\frac{1}{10}$

$P(a3=no|d2=no)=\frac{6}{10}$

$P(d2=yes|a1=40.0, a2=yes,a3=no)\propto P(a1=42.0|d2=yes)P(a2=yes|d2=yes)P(a3=no|d2=yes)P(d2=yes)=\frac{9}{10}\cdot\frac{0}{10}\cdot\frac{1}{10}\cdot\frac{10}{20}$

$P(d2=no|a1=40.0, a2=yes,a3=no)\propto P(a1=42.0|d2=no)P(a2=yes|d2=no)P(a3=no|d2=no)P(d2=no)=\frac{0}{10}\cdot\frac{1}{10}\cdot\frac{6}{10}\cdot\frac{10}{20}$

# Q3


![Q3-figure](flowchart.png){width=100%}

## (a)

$$\begin{aligned}P(\bar{A}, B, \bar{C}, D)&=P\big{(}\bar{A}|parents(\bar{A})\big{)}P\big{(}B|parents(B)\big{)}P\big{(}\bar{C}|parents(\bar{C})\big{)}P\big{(}D|parents(D)\big{)}\\&=P(\bar{A})P(B)P(\bar{C}|\bar{A})P(D|\bar{A},B)\\&=\big{(}1-P(A)\big{)}P(B)\big{(}1-P(C|\bar{A})\big{)}P(D|\bar{A},B)\\&=0.9\times0.5\times0.8\times0.6\\&=0.216\end{aligned}$$

## (b)



$$\begin{aligned}P(A|B,C,D)&=\frac{P(A,B,C,D)}{P(B,C,D)}\\&=\frac{P(D|A,B,C)P(A,B,C)}{P(D|B,C)P(B,C)}\\&=\frac{P(D|A,B)P(C|A,B)P(A,B)}{\big{(}\sum_AP(D|A,B,C)P(A)\big{)}P(C|B)P(B)}\\&=\frac{P(D|A,B)P(C|A)P(A)P(B)}{\big{(}\sum_AP(D|A,B)P(A)\big{)}\big{(}\sum_AP(C|A)P(A)\big{)}P(B)}\\&=\frac{0.9\times0.7\times0.1\times0.5}{(0.9\times0.1+0.6\times0.9)(0.7\times0.1+0.2\times0.9)\times0.5}\\&=0.4\end{aligned}$$
