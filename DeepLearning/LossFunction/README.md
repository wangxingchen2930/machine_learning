# Loss Function

## Cross-entropy
- commonly used in CNN
- example: 
><img src="https://latex.codecogs.com/gif.latex?{\begin{aligned}J(\mathbf%20{w}%20)\%20&=\%20{\frac%20{1}{N}}\sum%20_{n=1}^{N}H(p_{n},q_{n})\%20=\%20-{\frac%20{1}{N}}\sum%20_{n=1}^{N}\%20{\bigg%20[}y_{n}\log%20{\hat%20{y}}_{n}+(1-y_{n})\log(1-{\hat%20{y}}_{n}){\bigg%20]}\,,\end{aligned}}"/>
where <img src="https://latex.codecogs.com/gif.latex?{\hat%20{y}}"/> is predicted vallue while <img src="https://latex.codecogs.com/gif.latex?{y}"/> is true value