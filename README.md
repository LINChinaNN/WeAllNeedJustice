# WeAllNeedJustice

One of the Kaggle's top10 data scientist once had joined the Bimbo competition and was caught by cheating. This genius had written a kernel. The first line is "I used linear regression to fit coefficients", but the genius denied a suggestion of "exponentiating both sides in the final equation then it be solvable by LR" and concluded that "In general, this system of equations has no solution".
We know that a LR model looks like y=W^X+b, and the generalized linear model g(y)=W^X+b (^ represents T here). If we use LSM, and when X^X is a full-rank matrix, we can get W and b's closed-form solutions. If "In general, this system of equations has no solution", then maybe you are using a non-linear function and solve it by gradient descent or Newton method. They are two different methods. The genius had editted this kernel several times. Why the genius omitted this obvious typo?

The genius also wrote:
2017-10-02 09-18-21.png

It seems that min obj1 usually is not equal to obj2, but the equivalence happens not only when log(1+a*x1+b*x2+c)=y. For example, it can happen when sum(delta1^2) = constant*sum(delta2^2). It may has various conditions can satisfy this eqn. At least, a eqn like exp(y)-x = c*(x-log(x)), (here x>=1) may has not only one solution. This is commonsense. A top10 data scientist should never make such mistake.

We may wonder how can a genius who confuses the basic concepts of machine learning and lacks the basic knowledge of maths win so many competitions so easily? Once I had reported this genius may cheated at another competition, I only received many downvote, maybe some guys just wanted me shut up. None cared how I knew that, and how can I proved it. In fact, if you have chance to talk to this genius, you only need 10 or 5 mins, you will trust every word I said.
