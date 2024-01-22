# Explanation-of-code
---

##Task 1 Explanation 
---
  
###Q.why the console.log shows the older value of count ?
- Becuse the set `React.useState(0)` is asynchronous nature `js` is synchronous nature thats why when we console the value of `count ` it print older value of count.

- i think the `setCount ` call a api to update the value of count.


---
##Task 2 Explanation
---
###Q.explain why count value is not updated to 3 as expected

- Because in `React ` it's create the batch of process and then send in `queue` and then react start its work when we update the value `setCount(count +1)` in three times its make a batch and it go in queue and then when react start work in process react alwals take older value of count for all the process which comes in  one batch so it is reasoon count update oncly one time .This problem we can solve using `callBack ` function for example `setCount(prevValue()=>prevValue+1)`






