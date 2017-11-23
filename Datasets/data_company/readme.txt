!!! Copied from http://omen.cs.uni-magdeburg.de/itikmd/gfkl2005/ !!!

In the run up to the conference a data mining competition takes place, which is 
sponsored by the "Deutsche Sparkassen- und Giroverband" (DSGV).

Data Mining Competition

Prediction of the Liquidity Crisis of Companies

Companies getting into a liquidity crisis is one of the major problems banks 
have to face today. The goal of the competition is to predict a liquidity crisis
 based on (a subset of) 26 variables describing attributes of companies.

The data:

For the participation in the competition you need the file "data_company.zip".
After extraction you will find training and test data in the files 
"data_company_train.txt" and "data_company_test.txt" with a semicolon separating
the values.

The training data file has 20,001 lines:

    * The column names are given in the first line.
    * The following 20,000 lines contain the companies' data.

The training data file has 28 columns:

    * The first column is a unique identifier ("ID").
    * The second column ("Ereignisflag") encodes whether the company got into a
      liquidity crisis, where "1" indicates a crisis and "0" no crisis.
    * The following columns ("VAR01" to "VAR26") contain the values of the 26 
      variables that may explain the crisis. All 26 variables are metric.
      
            TYPE MISSING
      VAR01 DBL  0
      VAR02 DBL  0
      VAR03 DBL  0
      VAR04 DBL  2995
      VAR05 INT  0
      VAR06 DBL  0
      VAR07 DBL  1400
      VAR08 DBL  88
      VAR09 DBL  88
      VAR10 DBL  27742
      VAR11 DBL  0
      VAR12 DBL  24800
      VAR13 DBL  11729
      VAR14 DBL  0
      VAR15 DBL  0
      VAR16 DBL  88
      VAR17 DBL  24126
      VAR18 DBL  12604
      VAR19 DBL  24974
      VAR20 DBL  0
      VAR21 DBL  0
      VAR22 DBL  11729
      VAR23 DBL  15056
      VAR24 DBL  0
      VAR25 DBL  29826
      VAR26 DBL  0
      
The test data file has 10,001 lines and 27 columns:

    * The first column is a unique identifier ("ID").
    * The following columns ("VAR01" to "VAR26") contain the values of the 26 
      variables that may explain the crisis.
      The test data set has no binary flag indicating the class label.

The task:

Build a model to predict the liquidity crisis for the companies.
