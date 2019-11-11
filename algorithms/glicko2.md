# Glicko2

Glicko rating mainly has the following features.
- Each player has a "ratings reliability"(RD) in addition to ratings, and if the number of matches is small, RD value is high and the rating is considered unstable.
- If the RD value is high, the fluctuation range of the rating is large, and new player will quickly settle to the proper rating. And the effect for the opponent is smaller than elo.
- RD becomes smaller as the player gets a match, while RD increases again by each "rating period" for a certain time. This takes into consideration that player’s skill will change as time passes.

Glicko2 improves on the Glicko by incorporating the rating volatility "σ" factor.

[wiki](https://en.wikipedia.org/wiki/Glicko_rating_system) | [paper](http://www.glicko.net/glicko/glicko2.pdf)

- [python](https://github.com/sublee/glicko2/blob/master/glicko2.py)
- [nodejs](https://www.npmjs.com/package/glicko2)
- [R](https://github.com/Schw4rz/glicko2)
