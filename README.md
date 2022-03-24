# mongo-indexing-part-2
### Problem
#### Ques:~(i) explain what is indexing in simple analogy?
#### Ques:~(ii) why do we use it?
#### Ques:~(iii) explain in simple terms how indexing pros and cons.
#### Ques:~(iv) if you can explain a bit about the data structure used
#### Ques:~(v) what is compound indexing?
***Ans1:~***

- Indexes are special data structures [1] that store a small portion of the collection's data set in an easy to traverse form.
- Indexes support the efficient execution of queries in MongoDB.
-  Without indexes, MongoDB must perform a collection scan, i.e. scan every document in a collection, to select those documents that match the query statement. 
-  If an appropriate index exists for a query, MongoDB can use the index to limit the number of documents it must inspect.
-   The index stores the value of a specific field or set of fields, ordered by the value of the field.
