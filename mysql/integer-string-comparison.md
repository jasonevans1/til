# Mysql integer to string comparison.

Mysql converts the varchar to an int before doing the comparison. If you do not set the where condition to a string value you could get unexpected results. See the example gist below.

[Example gist](https://gist.github.com/brianr/4208061)
