# Database Consistency

## Eventually Consistency
* Use some rule to apply replicate data.
* Allow to request anytime, it possible for client to see conflict.
* Eventually all request will get same response.
* Example: last-write-wins in Distributed System
  * dataNodeA = 'foo'
  * dataNodeB = 'foo'
  * [A] write 'John' to dataNodeA
  * [B] write 'Doe' to dataNodeB
  * **Before resolve conflict**: [A] get 'John', and [B] get 'Doe'.
  * **After resolve conflict**: [A] and [B] will get 'Doe' when read.

## Strong Consistency
* Make sure new data available to every request access...

## Weak Consistency
* Not guarantee latest updated data to return for any access....
* Example:
  * A = 0
  * x write 1 to A
  * y Read A between x writing 1 to A.
  * y get 0

### References
* [Eventually Consistent](http://www.allthingsdistributed.com/2008/12/eventually_consistent.html): 
* [CAP Theorem](https://en.wikipedia.org/wiki/CAP_theorem): Problem about read/write data in Distribution System.
* [ACID](https://en.wikipedia.org/wiki/ACID):
  * Atomicity: Each transactions be "all or nothing", if pass all - save all, if fail some - rollback all.
* [Consistency Model](https://en.wikipedia.org/wiki/Consistency_model#Example)