#### example:
$$z ~ N(0,\sigma^2)$$
$$x_1 = z + N(0,1)$$
$$x_2 = z + N(0,1)$$

Then ridge regression tend to bring both $x_1$ and $x_2$ into the predictors with weight 1/2. consider the object function as follows
$$min \sum (\hat{y_i}-y_i)^2 + \lambda ||\beta||_2$$

2 case: 
* $\beta_1 = 1/2$; $\beta_2 = 1/2$ 
* $\beta_1 = 1$;   $\beta_2 = 0$
