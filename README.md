Learning Probability Density Function using Roll-Parameterized Non-Linear Model
This project implements a roll-number-parameterized non-linear transformation and learns a Gaussian Probability Density Function (PDF) using the **NO₂ feature** from the India Air Quality dataset.

Taking dataset from the source:https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data

Taking only the NO2 feature present in dataset

Step 1: Transformed each value of x into z using the transformation function

z = T_r(x) = x + a_r \sin(b_r x)
where r is university roll number
with ar = 0.05 ∗ (r mod 7), br = 0.3 ∗ (r mod 5 + 1)

Step-2: Learn parameters  probability density function using Maximum Likelihood Estimation (MLE)

p^​(z)=ce−λ(z−μ)2

Where, p̂(z) is the predicted probability of the transformed variable z.
Learning parameters λ, μ and c.
