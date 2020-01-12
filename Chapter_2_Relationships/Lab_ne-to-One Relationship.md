Lab: One-to-One Relationship
Problem:

A legacy database has been ported to MongoDB, resulting in a set of collections that were mapped to their original tables. This port has been quickly identified as a poor solution.

We have been tasked with redesigning the employees collection to make better use of the document model to make the information clearer.

![](https://university-courses.s3.amazonaws.com/M320/lab_relationship_one-to-one-problem.png)

While we are restructuring the database, the Human Resources department would like us to move any confidential employee information to a different collection to make the information easier to protect.

Consider the following potential schema designs. Each of these designs represents an individual employee and the One-to-One relationship between all of their fields.

The ideal schema design should store:

address information together as an embedded sub-document
all of an employee's phone numbers together as an embedded sub-document
all salary and bonus compensation information together as an embedded sub-document
all confidential information in a separate collection
Once you've identified the ideal design, you can deepen your knowledge by trying to explain why each of the other options is not the preferred design choice.

Attempts Remaining:3 Attempts left

Choose the best answer:

- [x] ![](https://university-courses.s3.amazonaws.com/M320/lab_relationship_one-to-one-answer-1.png)

- [ ] ![](https://university-courses.s3.amazonaws.com/M320/lab_relationship_one-to-one-answer-2.png)

- [ ] ![](https://university-courses.s3.amazonaws.com/M320/lab_relationship_one-to-one-answer-4.png)

- [ ] ![](https://university-courses.s3.amazonaws.com/M320/lab_relationship_one-to-one-answer-5.png)

- [ ] ![](https://university-courses.s3.amazonaws.com/M320/lab_relationship_one-to-one-answer-3.png)
