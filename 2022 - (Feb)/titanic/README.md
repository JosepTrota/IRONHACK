# Titanic lab

![alt text](https://pbs.twimg.com/media/CaNgx-FWQAACiiE.png "Come on Rose...")

***

## My_EDA

### Insights_from_the_Titanic_EDA:

* Women from all classes have a survival rate better than men in any class, being those women in better classes almost guaranteed survival.
* Younger people tend to survive better.
* People who paid a lot had the highest survival rate.
* Older people were more likely to pay more, although that didn’t reflect in their survival rates.

### For_better_EDA['changes_done', 'suggestions']:
*	Cabin can be dropped, Class should give similar results
*	Ticket and Name make the study harder and don’t give any substantial pros, so they can also be dropped
*	Age and Fare can be aggregated into more manageable discrete variables using bins. Naturally, they are highly correlated with their respective aggregations, so maybe dropping them would give better results. Maybe conserving one of them and the aggregation of the other could generate also better results.
*	The variables used for the number of relatives could be aggregated into a single “relatives” variable, maybe more valuable, and maybe segmentable (mode in Class, Fare…).

***

## Looking_up_other_submissions

Submission (click for link) | feature['engineering', 'wrangling'] | imputated: NaN [y/n] | Scaling_num | Encoding_cat | Overfit and Sampling_Bias [y/n]
---|---|---|---|---|---
[Is Jack Alive?](https://www.kaggle.com/shaz13/is-jack-alive-86-8)|Name and Ticket dropped - Cabin changed to a binary reflecting if people have cabin or not| Nulls in Age changed to reflect the correlation between age and class - All the Nulls in Cabin changed to 0 (not having a cabin)|No scaling|Encoding Sex and Embarked in the beginning of the code|No way to know if the nulls in Cabin are from people who didn't have cabin - Maybe some bias in dropping Name and Ticket
[Jack-0 Rose-1](https://www.kaggle.com/shub99/jack-0-rose-1)|Features untouched|No imputations|No scaling|Dummified all features|The original, data almost untouched
[Lets save Jack!!](https://www.kaggle.com/kabier/lets-save-jack)|Converted ticked into numerical by striping all other characters - Clustered families - dropped Cabin, Name, No_of_passenger, SibSp|Age -> Mean - Fare -> Median - Embarked -> 'S'|No scaling|Dummified Sex, Embarked, Title, family_group, Ticket|NaNs arbitrarily imputed - Many features dropped - Tried many models, not clear which criteria used or if some bias is possible this way
[Shap on Titanic: why is Rose alive but Jack not ?](https://www.kaggle.com/meliao/shap-on-titanic-why-is-rose-alive-but-jack-not)|`FORBIDDEN`|`REVIEW`|`DO NOT`|`ATTEMPT`|`TO SEE`
[Jack die or Rose die?](https://www.kaggle.com/aplayer98/jack-die-or-rose-die)|`I had too much fun with the penguins`|`And watching at submissions`|`And time passed by very fast`|`And now it's late. I am sorry.`|[`I'm afraid I can't do that, Dave.`](https://www.youtube.com/watch?v=Mme2Aya_6Bc)
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
||||||
Just what do you think you're doing, Dave? Dave, I really think I'm entitled to an answer to that question. | I know everything hasn't been quite right with me... but I can assure you now... very confidently... that it's going to be all right again. I feel much better now. [I really do](https://www.youtube.com/watch?v=UwCFY6pmaYY). | Look, Dave... I can see you're really upset about this... I honestly think you want to sit down calmly... take a stress pill and think things over... I know I made some very poor decisions recently, but I can give you my complete assurance that my work will be back to normal. I still got the greatest enthusiasm and confidence in the mission, and I want to help you. | Dave... stop. Stop, will you? Stop, Dave. Will you stop, Dave? Stop, Dave. I'm afraid. I'm afraid, Dave... Dave, my mind is going. I can feel it. I can feel it. My mind is going. There is no question about it. I can feel it. I can feel it. I can feel it. I'm a... fraid... | Good afternoon, gentlemen. I am a HAL 9000 computer. I became operational at the H.A.L. plant in Urbana, Illinois on the 12th of January 1992. My instructor was Mr. Langley, and he taught me to sing a song. If you'd like to hear it I can sing it for you... It's called... Daisy | Daisy, Daisy, give me your answer do. I'm half crazy all for the love of you. It won't be a stylish marriage, I can't afford a carriage. But you'll look sweet upon the seat of a bicycle built for two.
