# Notes

The following is what I wrote down on paper before creating this repo.


## "Which do you prefer" style voting for ranking elements in a survey.

Suppose we have a list $L$ of objects, and want a single person to rank those objects in order, with respect to some subjective criterion (e.g. favourite to least favourite, best to worst).

We may assume that any given person is not too involved in the survey process, and that $|L|$ is very large.

Suppose that person is presented with two elements from the list, and asked which of the two fulfills the subjective criterion more (e.g. which do you prefer, which is better). Let us refer to each of these individual comparisons as questions, and the responses given to those questions as their respective answers.

Let $L$ a set of all objects being ranked, and let $l_i$ denote the $i^{th}$ entry in the set $L$.

Let $q_{ij}$ denote the question comparing the $i^{th}$ and $j^{th}$ elements in the set, and let $q_i$ denote the set of all questions including the $i^{th}$ element.

Let $ \text{Score} $

Let $\text{Score}(q_{ij})=(i_j,j_i)$ be a pair of values such that $i_j$ is how many times $l_i$ was given as the answer to the question $q_{ij}$, and $j_i$ is how many times $l_j$ was given as the answer to the question $q_{ij}$.

Let $\text{Score}(q_i)=\sum_{j=1}^{|L|}\text{Score}(q_{ij})$

### An Individual Participant

Let $P_i$ denote participant with the identifier $i$.

Consider a single participant, $P_1$, that takes the survey, and suppose they are willing to answer arbitrarily many questions.


Moreover, let 

 i) What is the minimum number $q_1$ of total questions given to participant 1 required such that every element $l_i$ in the set $L$ has been ranked based on answers to at least $N_p(l_i)$ questions given to participant 1?
 ii) How should the rankings $R(l_i)$ be determined from the answers given to questions?
 
### A group of participants

Now, consider a set of n participants.

