# Predicting Book Purchases

## Situation

On Aug 1, 2014 a leading German book retailer sent out an offer to its customers. They observed the purchases that were made in response to this offer. Your task is to use information that was available to the company as of Aug 1, 2014 to construct a machine learning model that predicts the spending in response to the offer.

## Data

There are two files.

- `booktrain.csv`: This gives the dependent variable for the training set only. You should find 8311 records plus a header.

  - `id`: unique customer identifier
  - `logtarg`: dependent variable. It is the **natural** logarithm of the spending in response to an offer mailed on 01AUG2014.

- `orders.csv`: All orders prior to `01AUG2014` for training (n=8311) and test (n=25,402) sets. You should find 627,955 records plus a header.

  - `id`: unique customer identifier
  - `orddate`: order date
  - `ordnum`: order number
  - `category`: category identifier, 1=fiction; 3=classics; 5=cartoons; 6=legends; 7=philosophy; 8=religion; 9=psychology; 10=linguistics; 12=art; 14=music; 17=art reprints; 19=history; 20=contemporary history; 21=economy; 22=politics; 23=science; 26=computer science; 27=traffic, railroads; 30=maps; 31=travel guides; 35=health; 36=cooking; 37=learning; 38=games and riddles; 39=sports; 40=hobby; 41=nature/animals/plants; 44=encyclopedia; 50=videos, DVDs; 99=non books
  - `qty`: quantity
  - `price`: price paid

## Evaluation Metric

You will be evaluated on the RMSE of your predictions on a test set.
