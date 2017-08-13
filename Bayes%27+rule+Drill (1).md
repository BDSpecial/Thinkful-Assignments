
First look over the numbers and estimate each of the four probabilities, using your intuition. Then, calculate the probabilities using Bayes' rule.

A diagnostic test has a 98% probability of giving a positive result when applied to a person suffering from Thripshaw's Disease, and 10% probability of giving a (false) positive when applied to a non-sufferer. It is estimated that 0.5 % of the population are sufferers. Suppose that the test is now administered to a person whose disease status is unknown. Calculate the probability that the test will:

- P(Thripshaw | Positive Test) = 0.98 or 98%
- P(Thripshaw | Negative Test) = 0.02 or 2%
- P(No_Thripshaw | Positive Test) = 0.1 or 10%
- P(No_Thripshaw | Negative Test) = 0.9 or 90%
- P(Infected) = 0.005 or 0.5%
- P(Not_Infected) = 0.995 or 99.5%

P(A | B) = P(B | A) * P(A) / P(B)
or
P(A | B) = P(B | A) * P(A) / [P(A)*P(B|A) + P(A~)*P(B|A~)]
P(Infected| Positive Test) = P(Positive Test| Infected) * P(Infected) / P(Positive Test)
= .9999 * .000001/(.000001*.9999 + .999999*.0001) = .0099 or .99%

1. Be positive
- This question is asking what is the probabily of a positive test both if they have Thripshaw and if they don't have the disease. My first thought is that given there is a 98% positive result for people with the disease and a 10% positive result for those without the disease that the mean of both of these percentages would give me the likelihood of a positive result each time a test is administered. 98% + 10% / 2 = 54%. So there is a 54% that the test will be positive each time. 

Bayes' rule says:
----------------
P(Positive Test | Thripshaw) = 
_______________________________
P(Thripshaw | Positive Test) * P(Infected) /
____________________________________________
[P(Thripshaw | Positive Test) * P(Infected) + P(No_Thripshaw | Positive Test) * P(Not_Infected)]

= 0.98 * 0.005 / [0.98 * 0.005 + 0.1 * 0.995] = 0.0049 / [0.0049 + 0.0995] = 0.0049 / 0.1044 = 0.0469 or 4.69%

or 

P(Positive Test | No_Thripshaw) =
_______________________________
P(No_Thripshaw | Positive Test) * P(Not_Infected)/
__________________________________________________
[P(No_Thripshaw | Positive Test) * P(Not_Infected) + P(Thripshaw | Positive Test) * P(Infected)]

= 0.1 * 0.995 / [0.1 * 0.995 + 0.98 * 0.005] = 0.0995 / [0.0995 + 0.0049] = 0.0995 / 0.1044 = 0.9530 or 95.3%


2. Correctly diagnose a sufferer of Thripshaw's
- So what is the probabily of getting a positive test result for someone who truely has the disease? My inital thought is that if a person has the disease and the test has a 98% probability of giving a positive result when applied to someone with the diease the the probability is simply 98%.

Bayes' rule says:
----------------
P(Positive Test | Thripshaw) = 
_______________________________
P(Thripshaw | Positive Test) * P(Infected) / 
____________________________________________
[P(Thripshaw | Positive Test) * P(Infected) + P(No_Thripshaw | Positive Test) * P(Not_Infected)]

= 0.98 * 0.005 / [0.98 * 0.005 + 0.1 * 0.995] = 0.0049 / [0.0049 + 0.0995] = 0.0049/.1044 = 0.0469 or 4.69%

3. Correctly identify a non-sufferer of Thripshaw's
- So what is the probabily of getting a negative test result for someone who does not have the disease? My inital thought is that if the person does not have the diease but the test have a 10% false positive the there is a 90% change the the test correct identifies someone as not having the diease. 

Bayes' rule says:
----------------
P(Negative Test | No_Thripshaw) =
__________________________________
P(No_Thripshaw | Negative Test) * P(Not_Infected)/
__________________________________________________
[P(No_Thripshaw | Negative Test) * P(Not_Infected) + P(Thripshaw | Negative Test) * P(Infected)]

= 0.9 * 0.995 / [0.9 * 0.995 + 0.02 * 0.005] = 0.8955 / [0.8955 + 0.001] = 0.8955 / 0.8965 = 0.9988 = 99.88%

4. Misclassify the person
- What is the probability of either a Negative test for a person with Thripshaw disease or a false Positive test for someone who doesn't have the disease? My inital thought is that since there is a 2% chance of negative test for a person with Thripshaw and a 10% chance of a false positive for someone without the disease, then the mean of both of these percentages would give me the likelihood of a incorrect result each time a test is administered. 2% + 10% / 2 = 6% chance of incorrect results. 

Bayes' rule says:
----------------
P(Negative Test | Thripshaw) =
_______________________________
P(Thripshaw | Negative Test) * P(Infected)/
___________________________________________
[P(Thripshaw | Negative Test) * P(Infected) + P(No_Thripshaw | Negative Test) * P(Not_Infected)]

= 0.02 * 0.005 / [0.02 * 0.005 + 0.9 * 0.995] = 0.0001 / [0.0001 + 0.8955] = 0.0001 / 0.8956 = 0.00011166 = 0.0111657%

or 

P(Positive Test | No_Thripshaw) =
__________________________________
P(No_Thripshaw | Positive Test) * P(Not_Infected)/
__________________________________________________
[P(No_Thripshaw | Positive Test) * P(Not_Infected) + P(Thripshaw | Positive Test) * P(Infected)]

= 0.1 * 0.995 / [0.1 * 0.995 + 0.98 * 0.005] = 0.0995 / [0.0995 + 0.0049] = 0.0995 / 0.1044 = 0.9530 or 95.30%

