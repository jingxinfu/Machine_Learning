# Machine Learning

## 1.Bayesian
### 1.1Basic Introduction 
Commonly, when calculating probabilities of a specific event occurrence, we will come out its prior possibilities quickly. However, the answer is wrong in a lots of cases. For instance, there are two bowls and each of them contain two kinds of cookie, chocolate and vanilla.

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
         |Bowl 1|Bow2
---------|------|----
Chocolate|20|10
Vanilla  |20|30
 
**if we randomly chose a bowl and take out a vanilla cookies, what is the probabilities of the event that we take out the vanilla from bowl 1?**

Simply, we will thinks, well, it's definitely 1/2.
Yes, the prior probabilities is exactly 1/2. we have half chance to choose bow1. Given that we have already known that the cookies we take out is chocolate cookies, we must take it into consideration when we answer the question.

So here is how I thought:

1. we have half chance to choose each bowl: 
*P(bow1)=1/2*
2. Take out vanilla chocolate from bow1: *P(bow1 | vanilla)=1/2*
3. Take out vanilla chocolate from bow2: *P(bow2 | vanilla)=1/4*
4. Take out vanilla chocolate: *P(vanilla)=P(bow1 | vanilla) + P(bow2 | vanilla)=3/4*
5. **As P(A)P(A|B)=P(B)P(B|A) (if A and B are independent, bayesian)**
6. **P(vanilla)P(vanilla | bow1)=P(bow1)P(bow1 | vanilla)**
7. 

```math
 P(vanilla | bow1) = (1/2 * 1/2) / (3/4) = 1/3
```
