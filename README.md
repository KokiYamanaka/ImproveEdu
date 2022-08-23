**Description**

This notebook, I built a model to predict whether a given competitive math problem is either a algebra or a number theory topic.
2 models are being implemented. A LSTM and a simple neural network.
Each training data contains problem sentences, category, difficulty, and solutions.
The dataset contains 7 different categories of math problem and I extracted 2 of those.
we will use math problem sentences as our x input and the category as our y output label.

**Problem motivation**:

Many students found difficulty in studying mathematics. Most of the time, the difficulty happends because they do not know where or what to review when facing a math assignment. Thus, by tagging the topic on a math question they're facing to solve, it will improve the process of reviewing their materials.

**Single train data**: 

{
    "problem": "What is the coefficient of $x^8$ in the expansion of $(x-1)^9$?",
    "level": "Level 3",
    "type": "Counting & Probability",
    "solution": "By the Binomial Theorem applied to $(x+(-1))^9$, this term is $\\binom98x^8(-1)^1=-9x^8$.  The coefficient of this term is $\\boxed{-9}$."
}

**Dataset obtained from**: 
<br> https://github.com/hendrycks/math
