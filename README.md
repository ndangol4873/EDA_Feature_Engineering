# EDA_Feature_Engineering

## Basic Steps for EDA and Feature Enginerring 

#### 1. df.info() -- Basic Informaton of the Data set.
#### 2. df.describe() -- Descriptive Statical details of the numerical columns.
#### 3 df.isnull().sum(), [feature for feature in df.columns if df[feature].isnull().sum()>0] -- Attribute Null details.
#### 4. df.dtypes -- Data type details.
#### 5. df['column'].value_counts() -- Column value counts.
#### 6. df.select_dtypes(include=['object']).columns -- Categorial field detail.
#### 7. df.select_dtypes(include=['int64','float64']).columns -- Numerical field detail.
#### 8. df.groupby(['Aggregate rating', 'Rating color', 'Rating text']).size() -- Grouping Operation.
#### 9.df[['Country','Currency']].groupby(['Country','Currency']).size().reset_index() -- Grouping Operation into dataframe

#### Handelling Categorical feature Gender in to Numerical Feature
#### 10. ## Updating the Gender Column with M = 1 and F = 0 df.Gender = df.Gender.map({'F':0, 'M':1})