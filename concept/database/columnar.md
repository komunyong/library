# Database - Columnar Database

* Fast for big data, in case of calculating that need to be done in all row in database

### Example

|id|name|price|
|-|-|-|
|0001|apple|300|
|0002|banana|400|
|0003|orange|500|

If need to SUM all product price column, in traditional way. Row-oriented will travel for *9 blocks* (0001, apple, 300, 0002, banana, 400, 0003, orange, 500) cause it query as whole row. For Columnar Database will travel for *3 blocks* (300, 400, 500) and then calculate. Let's try to thin about big data that has more than billion rows and columns. This is reason of columnar that **good for calculating in big data**.

### References
[Columnar Database](https://datascience.stackexchange.com/questions/8244/what-makes-columnar-databases-suitable-for-data-science)
[Column Oriented DBMS](https://en.wikipedia.org/wiki/Column-oriented_DBMS)
