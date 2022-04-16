# GARCH-in-Bollinger-s-Band-strategy
*Project was made with Katarzyna Hasal as a final part of Machine Learning course. Every line of code is an effect of this team work.*

Short revision of the GARCH model  and its potential use in Bollinger's Band strategy.

## I. Quick summary
It was our introduction to the GARCH(p,q) model and understanding it fully can be seen as the main purpose here. We started with some analyses concerning the data (stocks of top 10 NASDAQ's companies) f.e. its potential to be use for the GARCH model. Next, after getting some intuitions from the Python's already made model, we created our own simple GARCH(1,1) with the use of gradient descent method (as proper mathematicians we decided to calculate all nessesary gradients by hand). Then, better model (final one) got created as a generalization of the previous one: with any given *p*, *q* parameters (*scipy* helped with the derivatives this time). We compared the results for all 3 approaches used before (Python's function together with our first and second one) and made some validations to pick best possible *p*, *q* for our data. Final part introduces basic Bollinger's Band strategies and tries swapping the moving standard deviation used in bands with GARCH predicted one. MA was also changed to Kalman's filter curve. Results were compared depending on the profit made from using the strategy on historical data.
All of the validation was made as an addition to GARCH model evaluation, therefore it has many flows such as not enough tests to make significant conclusions. We did not wanted to actually decide whether using GARCH volatility can increase profit in Bollinger's Band approach- everything was connected with the purpose of understanding and practicing new concepts.

*Note: More info about theoretical background and all steps is in the Colab file.*


