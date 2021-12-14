# Asymmetrical-Kappa
R function for calculating the asymmetric version of Kappa

The Kappa statistics is one of the most used interrater reliability measure. Unfortunatly it starts with the premise that both raters are equally potent in their rating abbility. In pratice, Kappa is often used, when this is NOT the case. 

I stumbled past this measurement when I read a paper, where Kappa was used to test for retest-reliability. The same person filled in the same questionnaire again after 24h. This is an asymmetrical situation, where the second "rater"/measurement is used to test against a "standard". While the first rating is considered to be "correct". 

To take this into account, Trald O. Kvalseth proposed a different measurement, the asymmetrical Kappa (A coefficient of agreement for niomal scales: an symmetric version of Kappa (1991), Educational and psychological measureement, 51, 95-101).


The R code provided here creates a function that calculates the asymmetrical Kappa value for any given x*x-dataframe of ratings. Data can be processed by the function either as absolute values (which are then converted by "prop.table()") or already as relative frequencies.


