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
> ***We do indexing to execute the query faster and in minimum read opeation***

> ***It is similar to the idexing of a book***

***Ans2:~***
- We do indexing to minimize the read opeations.
- So when do we indexing, it scan the documents which are relevent to give desired output.

***Ans3:~***
##### Pros Of indexes are:~ 
1. Indexes minimizes the read operation in the database.
2. Indexes reduces the total number of document scanned.
3.  it scan the documents which are relevent to give desired output.
4.  Time taken by the query to execute will be decreased.
##### Cons of the indexes are:~
1. Indexing basically uses internaly B-Tree Data Structure
2. Insertion, deletion and updation becomes very costly in B-Tree Data Structures because we can delete a key from any node-not just a leaf—and when we delete a key from an internal node, we will have to rearrange the node’s children. 

***Ans4:~***
1. index uses B-Tree data Sturcture internally. 


***Ans5:~***
If we create a index with multiple field or more than one field, it is called compound indexing.
