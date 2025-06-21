+++
title = "Batch Gradient Descent"
date = 2025-06-22T02:58:44+05:30
description = "It demostrates algorithm of machine learning for linear regression problems."
draft = true
toc = false
categories = ["Machine Learning"]
[[copyright]]
  owner = "Sagar Ladla"
  date = "2025"
  license = "cc-by-nc-sa-4.0"
+++

This `Gradient Descent Algorithm` simply uses the one variable polynomial equation of straight line i.e.,

> Y = &theta;<sub>0</sub> + &theta;<sub>1</sub> * x

- &theta;<sub>1</sub> : slope of line
- &theta;<sub>0</sub> : Y intercept of the line (i.e., From which Y-coordinate the line will pass)
      
### Computing `Hypothesis` function:
**hypothesis()** - computes predicted/hypothysed value of corresponding value of input feature (x), given by
> h<sub>&theta;</sub>(x) = &theta;<sub>0</sub> + &theta;<sub>1</sub> * x<sup>(i)</sup>

### Computing `Cost` or `Error` function:
**cost()** - computes the totalError of the straight line which is calculated as **`sum of squared error`** by:
> cost(&theta;<sub>0</sub>, &theta;<sub>1</sub>) = 1/2M * <sup>M</sup>&sum;<sub>(i=1)</sub> (h(x<sup>(i)</sup>) - y<sup>(i)</sup>)<sup>2</sup>
corresponds to
> __cost(&theta;<sub>0</sub>, &theta;<sub>1</sub>) = 1/2M * <sup>M</sup>&sum;<sub>(i=1)</sub> ((&theta;<sub>0</sub> + &theta;<sub>1</sub> * x<sup>(i)</sup>) - y<sup>(i)</sup>)<sup>2</sup>__

### Computing `GradientDescent`:
#### To compute gradient descent we need to find the partial derivative of &theta;<sub>0</sub> and &theta;<sub>1</sub> individually
- <u>Formula to compute &theta;<sub>0</sub>'s partial derivative </u>
> &part; / &part; &theta;<sub>0</sub> = 1 / M * <sup>M</sup>&sum;<sub>(i=1)</sub> ((&theta;<sub>0</sub> + &theta;<sub>1</sub> * x<sup>(i)</sup>) - y<sup>(i)</sup>)

- <u>Formula to compute &theta;<sub>1</sub>'s partial derivative </u>
> &part; / &part; &theta;<sub>1</sub> = 1 / M * <sup>M</sup>&sum;<sub>(i=1)</sub> ((&theta;<sub>0</sub> + &theta;<sub>1</sub> * x<sup>(i)</sup>) - y<sup>(i)</sup>) * x<sup>(i)</sup>

<h5><pre>while convergence:<br>
       &theta;<sub>0</sub> = &theta;<sub>0</sub> - &alpha; * 1/M * <sup>M</sup>&sum;<sub>(i=1)</sub> ((&theta;<sub>0</sub> + &theta;<sub>1</sub> * x<sup>(i)</sup>) - y<sup>(i)</sup>)<br>
       &theta;<sub>1</sub> = &theta;<sub>1</sub> - &alpha; * 1/M * <sup>M</sup>&sum;<sub>(i=1)</sub> ((&theta;<sub>0</sub> + &theta;<sub>1</sub> * x<sup>(i)</sup>) - y<sup>(i)</sup>) * x<sup>(i)</sup><br>
       return [&theta;<sub>0</sub>, &theta;<sub>1</sub>]</pre></h5>
      
#### epcohs is simply the number of iterations we want to make over the whole dataset repetatively.
#### &alpha; is simply the learning rate of the gradient descent function (hyperparameter).

###### * Hperparameter - parameters which indirectly affect the <u>rate of iterations</u> or <u>learning algorithm</u> over the dataset.

-> [C++ implementation of the algorithm](https://github.com/sagarladla/everyting_c-cxx/blob/main/gradient-descent/gradient-descent.cpp)
