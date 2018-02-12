# ebkickers
Empirical Bayes Estimation for NFL Kickers - modeled after http://varianceexplained.org/r/empirical_bayes_baseball/

# Where's the Data?
Since I don't own the rights to the data, I can't share it here.

The csv file headers are:
```Rk,Player,Team,Pos,FGM,FG Att,Pct,Blk,Lng,A-M,Pct,A-M,Pct,A-M,Pct,A-M,Pct,A-M,Pct,XPM,XP Att,Pct,Blk```
which was copied from [NFL.com](http://www.nfl.com/stats/categorystats?archive=false&conference=null&statisticPositionCategory=FIELD_GOAL_KICKER&season=2017&seasonType=REG&experience=&tabSeq=1&qualified=false&Submit=Go).

Though ultimately I only care about Player, FGM (Field Goals Made), and FG Att (Field Goal Attempts).

Future iterations (following David Robinson's multinomial posts) may include data about field goal and distances (eg: Miss / 1-20 / 20-30 / 30-40 / 40-50 / 50+), but for now we're working with binomial data.