# Ranking

Ranking or Scoring or Rating all represent a specific pattern or sorting individuals or objects in a particular order according to a select criteria.

Learn here what [Wikipedia](https://en.wikipedia.org/wiki/Ranking) has on this.

### The Story

Consider you are rank mangoes.
Without any set basis, it's impossible to rank. But if you're given a base, say on size, color, sweetness, anything that's measurable. The ranking gets much easier.
What if you're to rank based on a combination of these. It gets a little complicated but still not impossible. You can first rank according to say sweetness and then size and then probably do an average of them as an easiest process. Is that the best available way to do it? Of course, NOT. But it's still allowed. In an ideal scenario the rank won't change much between various criteria as given.
For a short amount of data you can sort and rank them by yourself.

What if we're to rank all the cricket/soccer players? Based on runs/goals they scored, based on time on field, etc they can be ranked.
But this logic fails on a larger scale. So, we need a better way to do it.

Introducing Elo rating system.
The Elo rating system is a method for calculating the relative skill levels of players in zero-sum games such as chess. You can use a wide variety of criteria as denominator to classify or rank each object in a certain way. The relative scoring is the best way to ensure the scores of each participant will be help on for the longest part of time.

A modified version of Elo came with [Glicko](http://glicko.net/ratings/glicko.pdf) which later got further modified to [Glicko2](http://glicko.net/ratings/glicko2desc.pdf). (You can find the links to implementation below.)
Glicko2 starts with a median score of usually 1500 and ranks or plays games amongst other object/entity based on said denominators or criteria till the score settles down on each criteria. Each combination is also a different match between entity-object and entity-entity or object-object or object-entity. Of course as you can guess, the order/direction matters to an extent. (Not in all cases).

#### A few case studies:
- [Improve tennis rating system based on Glicko-2 system.](https://medium.com/@taiga_tachibana/improve-tennis-rating-system-based-on-glicko-2-system-d481e83a1ecb)


Our goal here is get to a modified state of glicko2 to bring up our own ranking algorithm to satisfy all said cases with minimum intervention. We'll go through all pros and cons of glicko2 algortihm and other ranking algorthims and come up a best feasible way, optimised to performance and speed of ranking.


### Various rating algorithms

- Elo
- [Glicko / Glicko-2](https://github.com/anistark/scoring/blob/master/algorithms/glicko2.md)
