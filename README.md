# Abstract RPG Rules

## Introduction

In RPGs, most gameplay does not need rules.  During play, players will only recurr to rules in two instances:
1. The gameworld is alien enough that *common sense* cannot be used to resolve a situation.  This is the case for magic spell casting, for instance.
2. Players do not want to determine the outcome according to their common understanding but want some undeterministic influence, i.e. chance, to do it for them.  This may be used to enhance tension or drama but also to reolve different understanding of the situation by different players, but they can still agree on a chance value.

All rule systems on the market (that I know of) do not separate the two points sufficiently and create probabilities that are hard to gauge. In fact, only for playing a game for an extended period of time, will patterns emerge. I find this fatiguing, in particular, if the probabilities do not turn out to match expectations and thereby impacting enjoyment. Therefore the following rules are written with these points in mind:
1. Keep out rules that explain a setting. I call these *in-world* rules.
2. Keep it comprehensible. This does not mean generic *simple*, but rather that probabilities do not provide surprises around the corner.

## Translation

Most rules intend to resolve skill application. Whether it be fighting, hiding, finding, lifting, or else. A character can have different skill levels but tasks at hand can also have different difficulty levels. We make the following assumptions: A skill proficiency and a task difficulty can be expressed as numbers. A skill level of *n* has the same chances of success for a task of difficulty *k*, as a skill of *n+1* against a difficulty of *k+1*. The numbers *n, k* are your regular numbers. Assuming we have a failure probability of *p* for a skill of *1* for a task of *0*. Then we *define* the skill value *2*, such that its failure probability for a task of *0* is *p<sup>2</sup>*. For simplicity sake, we will restrict ourself in the number range for $n, k$ and take $p=0.8$.

This is in fact all we need, because the following are conclusions. You do not need understand the above paragraph nor do you need to follow through with a rigorous proof. We will explain the actual rule(s) in more detail.

## On Rule to Rule them

You roll a *d5* until you roll a 1 and the count the number of dice that did not show up a 1. That is the same as the number of dice you actually rolled minus one. The higher you get, the better, therefore we call it the positive roll. This roll is dominated by the active character, or more generally, the actor. It should be clear in almost all situations, who is active - the one with the applicable skill. Of course, there is a negative roll that is associated with the passive resistance or impediment, which is handled in the same way. That would be the task in most cases. These two numbers are subtracted. An understanding of this rule is crucial, so we elaborate by listing the probabilities involved as well as some examples. If the method is intuitively clear, you can skip the (theretical) next section.

The mechanism is different from other rules, where you will often roll eithe a pool of dice and count those that match a certain threshold or single die roll gives you better results the higher (lower) your roll turns out.

In the following table the first row shows the result achieved when you roll. The second row shows the chance that you have of moving up one point (i.e. left) at any given point. Note that this chance is always the same. The third row gives the percentage chance that you have of achieving the result in the corresponding first row. These you could achieve by rolling a *d100* in order to cut down on the number of dice to roll. All but the first column of this row are approximations.

The last column is somewhat special. It combines all higher results. You could expand the table to infinity, if you wanted. While the extensions of the first and second row are quite obvious, the third is not. It should be interpreted thus: if you roll *91-100*, you need to roll again on this table, get the result as before and then add *10* to the result. (For the mathematically inclined, this is a recursive definition, since it is possible that you roll *91-100* again, which forces you to roll on this table again and add *20* to the net result from the repeated application. We will see this in the examples.)

| 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | ... |
| 80% | 80% | 80% | 80% | 80% | 80% | 80% | 80% | 80% | 80% | ... |
|01-20|21-36|37-49|50-60|61-68|69-74|75-80|81-84|85-87|88-90|91-100|

The previous table only considered one roll, the positive or the negative roll. (You can also call them the active and the passive roll; in most instances the obstacle is passive, such as door being lock-picked or a weight being lifted.) The following table shows the chances for overall results. Generally, this table is interpreted as the one above, with a few key differences.

With a roll of 01-06 and 95-100 the extended roll is continued on the previous table with the obvious consequences. Positive continuation is correct, while negative continuation results in negative results to be added. The second row cell below the 0 result means 4/9 chance to increase the result by 1, the same chance to descrease the result by one and a 1/9 to stay at 0. The astute reader will see the chance for 0 in the third row is only 8%, while 1/9 is approximatly 11%. Again this is due to rounding; the price for rolling less dice.
Table 2 ...	-9	-8 	-7	-6	-5 	-4	-3	-2 	-1	0	1 	2	3	4 	5	6	7 	8	9	...
...	80%	80% 	80%	80%	80% 	80%	80%	80% 	80%	44%/44%	80% 	80%	80%	80% 	80%	80%	80% 	80%	80%	...
01-06	07-08	09-10	11-12 	13-15	16-19	20-24	25-30 	31-37	38-46	47-54	55-63 	64-70	71-76	77
