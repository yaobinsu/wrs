DESCRIPTIONS OF DATA FILES
==============================================

Here are brief descriptions of the project data.

The full data set (train.data + test.data) contains 41,493 ratings by 5,681 users on 4,530 books.
Each user has rated at least 3 books. 
Each book has been rated by at least 3 users. 

train.data and test.data both contain the following fields:

user_id: the ID of the user that gave the rating
book_id: the ID of the book that was given the rating
review_id: the ID of the rating action
rating: the rating given by user_id to book_id, integer 1-5.
timestamp: the time when the rating was last updated (yyyy-mm-dd hh-mm-ss)

user_id, book_id, and review_id remain consistent with the IDs in the book.csv file.

The train.data and test.data are 80%/20% splits per user, based on timestamp.

The given book descriptions in book.csv have been automatically detected to be in English.
There may be some extra book_id in book.csv that do not exist in train.data/test.data.