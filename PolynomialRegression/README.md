# Sometimes, the trend of data is not really linear, and looks curvy. In this case we can use Polynomial regression methods. In fact, many different regressions exist that can be used to fit whatever the dataset looks like, such as quadratic, cubic, and so on, and it can go on and on to infinite degrees.

# In essence, we can call all of these, polynomial regression, where the relationship between the independent variable x and the dependent variable y is modeled as an nth degree polynomial in x. Lets say you want to have a polynomial regression (let's make 2 degree polynomial):

# 𝑦=𝑏+𝜃1𝑥+𝜃2𝑥2

# Now, the question is: how we can fit our data on this equation while we have only x values, such as  Engine Size? Well, we can create a few additional features: 1, 𝑥
# , and 𝑥2

# .

# PolynomialFeatures() function in Scikit-learn library, drives a new feature sets from the original  feature set. That is, a matrix will be generated consisting of all polynomial combinations of the  features with degree less than or equal to the specified degree. For example, lets say the original  feature set has only one feature, ENGINESIZE. Now, if we select the degree of the polynomial to be 2, then it generates 3 features, degree=0, degree=1 and degree=2: 

# It looks like feature sets for multiple linear regression analysis, right? Yes. It Does. Indeed, Polynomial regression is a special case of linear regression, with the main idea of how do you select your features. Just consider replacing the 𝑥 with 𝑥1, 𝑥21 with 𝑥2

# , and so on. Then the 2nd degree equation would be turn into:

# 𝑦=𝑏+𝜃1𝑥1+𝜃2𝑥2

# Now, we can deal with it as a 'linear regression' problem. Therefore, this polynomial regression is considered to be a special case of traditional multiple linear regression. So, you can use the same mechanism as linear regression to solve such problems. 