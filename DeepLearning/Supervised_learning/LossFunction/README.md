# Loss Function

## Cross-entropy
- commonly used in CNN
- example: 
><img src="https://latex.codecogs.com/gif.latex?{\begin{aligned}J(\mathbf {w} )\ &=\ {\frac {1}{N}}\sum _{n=1}^{N}H(p_{n},q_{n})\ =\ -{\frac {1}{N}}\sum _{n=1}^{N}\ {\bigg [}y_{n}\log {\hat {y}}_{n}+(1-y_{n})\log(1-{\hat {y}}_{n}){\bigg ]}\,,\end{aligned}}"/>
where <img src="https://latex.codecogs.com/gif.latex?{\hat {y}}"/> is predicted vallue while <img src="https://latex.codecogs.com/gif.latex?{y}"/> is true value