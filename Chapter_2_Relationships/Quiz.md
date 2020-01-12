# Chapter 2: Relationships

## Relationship Types and Cardinality

Problem:

Why did we introduce the one-to-zillions relationship in our modeling notation?
Attempts Remaining:∞Unlimited Attempts

Check all answers that apply:

- [x] **To address the fact that the concept of relationship linked to a huge number of entities is missing in normal crow's foot notation.**

- [ ] To address the fact that a crow's foot has 5 fingers, not 3.

- [x] **To highlight the fact that huge cardinalities may impact design choices.**

## One-to-Many Relationship

Problem:

Consider a one-to-many relationship observed between a county and the cities in that county.

Which of the following are valid ways to represent this one-to-many relationship with the document model in MongoDB?

Attempts Remaining:∞Unlimited Attempts

Check all answers that apply:

- [x] **Have a collection for the counties and a collection for the cities with each city document having a field to reference the document of its county.**

- [ ] Embed all the fields for a city as a subdocument in the corresponding county document.

- [x] **Embed the entities for the cities as an array of sub-documents in the corresponding county document.**

## Many-to-Many Relationship

Problem:

Consider a many-to-many relationship observed between movies and the actors starring in these movies, for a system that could provide detailed information about either a movie or an actor.

![](https://university-courses.s3.amazonaws.com/M320/rst-images-prob_movies_actors.png)

Which of the following are true about modeling this many-to-many relationship with the document model in MongoDB?

Attempts Remaining:∞Unlimited Attempts

Check all answers that apply:

- [x] **Embedding actors in movies still requires a separate collection to store all actors.**

- [ ] When using one collection for movies and one collection for actors, all movie documents must have an array of references to the actors in that movie, and all actor documents must have an array of references to the movies they appear in.

- [x] **Embedding actors in movies creates duplication of actor information.**

## One-to-One Relationship

Problem:

Which of the following are valid ways to represent a one-to-one relationship with the document model in MongoDB?
Attempts Remaining:Correct Answer

Check all answers that apply:

- [x] **Embed the fields as a sub-document in the document.**

- [x] **Link to a single document in another collection.**

- [x] **Embed the fields in the document.**

## One-to-Zillions Relationship

Problem:

Which of the following statements are true about one-to-zillions relationships?
Attempts Remaining:∞Unlimited Attempts

Check all answers that apply:

- [x] **The relationship representations that embed documents are not recommended.**

- [x] **We must take extra care when writing queries that retrieve data on the zillions side.**

- [x] **It is a special case of the one-to-many relationship.**
