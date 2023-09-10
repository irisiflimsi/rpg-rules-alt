# Abstract RPG Rules

## Introduction

In RPGs, most gameplay does not need rules.  During play, players will only recurr to rules in two instances:
1. The gameworld is alien enough that *common sense* cannot be used to resolve a situation.  This is the case for magic spell casting, for instance.
2. Players do not want to determine the outcome according to their common understanding but want some undeterministic influence, i.e. chance, to do it for them.  This may be used to enhance tension or drama but also to reolve different understanding of the situation by different players, but they can still agree on a chance value.

All rule systems on the market (that I know of) do not separate the two points sufficiently and create probabilities that are hard to gauge. In fact, only for playing a game for an extended period of time, will patterns emerge. I find this fatiguing, in particular, if the probabilities do not turn out to match expectations and thereby impacting enjoyment. Therefore the following rules are written with these points in mind:
1. Keep out rules that explain a setting. I call these *in-world* rules.
2. Keep it comprehensible. This does not mean generic *simple*, but rather that probabilities do not provide surprises around the corner.

## Translation

Most rules intend to resolve skill application. Whether it be fighting, hiding, finding, lifting, or else. A character can have different skill levels but tasks at hand can also have different difficulty levels. We make the following assumptions: A skill proficiency and a task difficulty can be expressed as numbers. A skill level of *n* has the same chances of success for a task of difficulty *k*, as a skill of *n+1* against a difficulty of *k+1*. The numbers *n, k* are your regular numbers. Assuming we have a failure probability of *p* for a skill of *1* for a task of *0*. Then we *define* the skill value *2*, such that its failure probability for a task of *0* is *p<sup>2</sup>*. For simplicity sake, we will restrict ourself in the number range for $n, k$ and take $p=0.8$. We also choose the chance for failure and success to be *50% = 1/2$ when *n = k = 0*.

This is in fact all we need, because the following are conclusions. You do not need to understand the above paragraph let alone follow a rigorous proof. We will explain the actual rule(s) as they affect the game in more detail.

## On Rule to Rule them

You roll a *d5* until you roll a 1 and the count the number of dice that did not show up a 1. That is the same as the number of dice you actually rolled minus one. The higher you get, the better, therefore we call it the positive roll. This roll is dominated by the active character, or more generally, the actor. It should be clear in almost all situations, who is active - the one with the applicable skill. Of course, there is a negative roll that is associated with the passive resistance or impediment, which is handled in the same way. That would be the task in most cases. These two numbers are subtracted. An understanding of this rule is crucial, so we elaborate by listing the probabilities involved as well as some examples. If the method is intuitively clear, you can skip the (theretical) next section.

The mechanism is different from other rules, where you will often roll eithe a pool of dice and count those that match a certain threshold or single die roll gives you better results the higher (lower) your roll turns out.

In the following table the first row shows the result achieved when you roll. The second row shows the chance that you have of moving up one point (i.e. left) at any given point. Note that this chance is always the same. The third row gives the percentage chance that you have of achieving the result in the corresponding first row. These you could achieve by rolling a *d100* in order to cut down on the number of dice to roll. All but the first column of this row are approximations.

The last column is somewhat special. It combines all higher results. You could expand the table to infinity, if you wanted. While the extensions of the first and second row are quite obvious, the third is not. It should be interpreted thus: if you roll *91-100*, you need to roll again on this table, get the result as before and then add *10* to the result. (For the mathematically inclined, this is a recursive definition, since it is possible that you roll *91-100* again, which forces you to roll on this table again and add *20* to the net result from the repeated application. We will see this in the examples.)

| 0     | 1     | 2     | 3     | 4     | 5     | 6     | 7     | 8     | 9     | ...   |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | ...   |
| 01-20 | 21-36 | 37-49 | 50-60 | 61-68 | 69-74 | 75-80 | 81-84 | 85-87 | 88-90 | 91-100|

The previous table only considered one roll, the positive or the negative roll. (You can also call them the active and the passive roll; in most instances the obstacle is passive, such as door being lock-picked or a weight being lifted. Or call them skill and task roll.) The following table shows the chances for overall results. Generally, this table is interpreted as the one above, with only a few key differences.

With a roll of *01-06* and *95-100* the extended roll is continued on the previous table with the obvious consequences. Positive continuation is correct, while negative continuation results in negative results to be added. The second row cell below the *0+ result means *4/9* chance to increase the result by *1*, the same chance to descrease the result by one and a *1/9* to stay at *0*. The astute reader will see the chance for *0* in the third row is only *8%*, while *1/9* is approximatly *11%*. Again this is due to rounding; the price for rolling less dice.

| ...   | -9    | -8    | -7    | -6    | -5    | -4    | -3    | -2    | -1    | 0       | +1    | +2    | +3    | +4    | +5    | +6    | +7    | +8    | +9    | ...    |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:   | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:  |
| ...	  | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 44%/44% | 80%   | 80%	  | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | 80%   | ...    |
| 01-06 | 07-08 | 09-10 | 11-12 | 13-15 | 16-19 | 20-24 | 25-30 | 31-37 | 38-46 | 47-54   | 55-63 | 64-70 | 71-76 | 77-81 | 82-85 | 86-88 | 89-90 | 91-92 | 93-94 | 95-100 |


### Examples

The most generic way to roll the dice would be to roll *d5* until a *1* is rolled. To improve speed, several *d10* may be rolled in ordered fashion. Order them according to size or alphabetical color (e.g. black, blue, green, yellow) or in any other way you can remember. With a *d10* stop at *1* or *2*. If you lack *d5*s (which are in fact *d10* where you half the resut and round up) you can also roll *d6*s with only a marginal *3%* error on each roll. But all players (and GM) should roll the same type dice. Computer applications that make rolling as easy as pressing a button are also easy to program.

- Assume you decided to use *d100* and rolled a *24* on the first roll. This means a result of *1* on the first table. The second roll (the negative or passive roll) shows a face *50*, which results in *3* on the first table for a net result of *-2*.

- Another decision is to use the combined table, and a *28* is rolled, which results in *-3*.

- A more exotic roll would be the sequence *96, 99, 93, 61* on the *d100*. The result would be *34*.

- Using the standard method, the positive sequence on a *d10* shows *3, 8, 10, 7, 9, 4, 6, 3, 10, 10, 8, 4, 2* and the negative sequence shows *3, 6, 9, 4, 4, 1*. The result is positive *12* and negative *5* with a net result of *+7*.

- If you decide that *+7* is not precise enough, a roll of *3* and *5* on a *d10* (each) gives are finer result of *+7.35*. I.e. you simple roll the decimal places.

Remember that the second row is technically correct and the third row only provides less rolls. We will look at some further hints for rolling.

### Hints

The calculations result in a level difference between the active and the passive part (or the skill level and task level) which is the only number relevant for rolling. If only the failure or success is of interest and not the success/failure level itself, you can apply the following shortcut. Since the difference must be met by the lower contestant, you may roll all the difference dice in one combined “throw” and check, whether any stop digit appears. If it does the lower contestant cannot win, since it is irrelevant, where the stop digit appears. If the stop digit does not appear, chances have reduced to 50/50, and you can flip a coin in any of a number of ways.

For example, suppose the active climber with a skill level of *57* wants to scale a cliff of difficulty *49*. The difference is *8*. The GM rolls *8* dice, which show up *3, 5, 6, 1, 3, 9, 9*, and *8*. Since *1* is a stop digit, the cliff is scaled. If the *1* had been a *7*, for instance, the cliff would have had a “fighting chance” to drop the character. The GM decides that even is good for the character and odd is bad and rolls a *d10*. It comes up a *6* and the character has barely made it. Any story-telling description of this close encounter is at your option.

Another pragmatic rule is rolling *10* non-stop rolls in a row can be shortened to rolling a *1* on a *d10*. The chance $1/10$ is an approximation of $0.8<super>10</super>$. You probably should use this, whenever the level differenc is at least *10*.  In fact, the choice of *p=0.8* in the initial paragraph was made for the reason that this heuristic holds.

## Applications to Existing Rules

Many rulesets rank a skill on a percentile scale *0%* through *100%*. This is the case for Rolemaster, Runequest, or Harnmaster. Rolling below your skill value makes you succeed. This approximates levels *0, 10, 20* and *30* at about *5%, 35%, 65%*, and *95%*. That means these rules have about fourty skill levels, in which all values fall according to our rules. The same is true for Dungeons and Dragons, Pathfinder, or the *d20* group of rules, which use twenty 5% steps, instead of the finer grained 1% step.

Note that you could just multiply the *d20* skill levels by two or take half for the precentile system, why the strange, non-linear mapping? Since we do not intend to simulate other rules in this manner, you most certainly can do that conversion. If, however, you intend to approximate the original probabilities, you should stick to the "strange" conversion.

The character sheet is applicable to all rules, because it captures the *out-world* probabilities. You need to fill in the relevant skills and tasks for the PC. Since the possible combinations are virtually limitless, list only the most common ones or add another sheet, if you do not find a suitable decomposition of skills and tasks.

Most rules apply linear modifications (i.e. additions and subtractions) to the skill and task levels and this is what we do for specific rule conversions in the dedicated sections.
