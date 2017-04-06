#### example1:
$$z ~ N(0,\sigma^2)$$
$$x_1 = z + N(0,1)$$
$$x_2 = z + N(0,1)$$

Then ridge regression tend to bring both $x_1$ and $x_2$ into the predictors with weight 1/2. consider the object function as follows
$$min \sum (\hat{y_i}-y_i)^2 + \lambda ||\beta||_2$$

2 case: 
* $\beta_1 = 1/2$; $\beta_2 = 1/2$ 
* $\beta_1 = 1$;   $\beta_2 = 0$

#### example2         
Lasso regression vs ridge regression
* ridge regression has less motivation to lower the beta (this point can explain the second point)
* Lasso works well for feature selection (to get rid of some unrelavent variables)
* Ridge works well for correlation features (combine some relavent variables)
refer the pics in P10. since the shape is like a square so the optimal point has more possibility to be a point...


#### LARS (basically replace Lasso)
A way to save time to choose right $\lambda$ in Lasso. Basically you only fit the data once and get a plot and choose the right $\lambda$                          
http://statweb.stanford.edu/~tibs/ftp/lars.pdf                           
http://www.cis.hut.fi/Opinnot/T-61.6040/presentations_s06/LARS.pdf


#### k-means
k-means algo is not fit for high r square situations.
