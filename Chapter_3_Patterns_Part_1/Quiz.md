# Guide to Homework Validation

Please follow the steps outlined in this lecture and included in the lecture notes.

To run the validator for the example lab on Windows, run the following command:

validate_m320 example --file answer_schema.json

To run the validator for the example lab on MacOS and Linux, run the following command:

./validate_m320 example --file answer_schema.json

Then, paste the validation code from the example lab into the text box below and hit the submit button.

**5d124f9bd971a774b97b5fc7**

## Handling Referential Integrity

Problem:

Which of the following are valid concerns regarding duplication, staleness and referential integrity management in a MongoDB database and appropriate resolution techniques?
Attempts Remaining:Correct Answer

Check all answers that apply:

-[x] **Data staleness issues can be minimized with frequent batch updates.**

-[ ] Data duplication should not exist and can be avoided with multi-document transactions.

-[x] **Data integrity issues can be minimized by using multi-document transactions.**

## Attribute Pattern

Problem:

Which one of the following scenarios is best suited for the application of the Attribute Pattern?
Attempts Remaining:∞Unlimited Attempts

Choose the best answer:

-[x] **Some fields share a number of characteristics, and we want to search across those fields.**

-[ ] The system is accessing the disk too frequently.

-[ ] The working set does not fit in memory.

-[ ] The documents are large.

-[ ] The documents need strict validation.

## Extended Reference Pattern

Problem:

Which one of the following scenarios is the best candidate to use the Extended Reference Pattern to avoid doing additional reads through joins/lookups?
Attempts Remaining:∞Unlimited Attempts

Choose the best answer:

- [ ] An app needs to retrieve a product and its ten most recent reviews.

- [ ] A product model needs to store references to images of the product that are kept in an external location outside the database.

- [ ] A product model needs to store a counter representing the number of times it was purchased.

- [ ] An order model needs to store the product ID, the price sold, and the quantity ordered for each product in an order.

- [x] **An app needs to retrieve a product and information about its supplier.**

## Subset Pattern

Problem:

Which one of the following scenarios is the best candidate for use of the Subset Pattern?
Attempts Remaining:Correct Answer

Choose the best answer:

-[x] **The working set does not fit in memory and it is difficult to scale the hardware.**

-[ ] The system is running out of RAM.

-[ ] The developers of the system have left and no one understands the application.

-[ ] The system is accessing the disk too frequently

-[ ] The documents are too big.

