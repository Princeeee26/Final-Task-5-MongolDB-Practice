# Final Task 6 MongolDB Practice
In this activity, we used MongoDB to insert, query, update, and delete documents within collections. Tasks included inserting movie data, performing text searches, managing relationships across users, posts, and comments, and executing complex queries to retrieve and manipulate related data.
## Part 1
- Create database

![screenshot](/Images/Database.jfif)

- Insert Documents

Queries:

![screenshot](/Images/Queries.jfif)

Output:

![screenshot](/Images/Output.jfif)

- Query / Find Documents

1. Get all documents

![screenshot](/Images/01.jfif)

2. Get all documents with `writer` set to "Quentin Tarantino"

![screenshot](/Images/03.jfif)

3. Get all documents where `actors` include "Brad Pitt"

![screenshot](/Images/05.jfif)

4. Get all documents with `franchise` set to "The Hobbit"

![screenshot](/Images/07.jfif)

5. Get all movies released in the 90s

![screenshot](/Images/09.jfif)

6. Get all movies released before the year 2000 or after 2010

![screenshot](/Images/11.jfif)

- Update Documents

1. add a synopsis to "The Hobbit: An Unexpected Journey" : "A reluctant hobbit, Bilbo Baggins, sets out to the Lonely Mountain with a spirited group of dwarves to reclaim their mountain home - and the gold within it - from the dragon Smaug."

![screenshot](/Images/13.jfif)

2. add a synopsis to "The Hobbit: The Desolation of Smaug" : "The dwarves, along with Bilbo Baggins and Gandalf the Grey, continue their quest to reclaim Erebor, their homeland, from Smaug. Bilbo Baggins is in possession of a mysterious and magical ring."

![screenshot](/Images/14.jfif)

3. add an actor named "Samuel L. Jackson" to the movie "Pulp Fiction"

![screenshot](/Images/15.jfif)

- Text Search

1. find all movies that have a synopsis that contains the word "Bilbo"

![screenshot](/Images/16.jfif)

2. find all movies that have a synopsis that contains the word "Gandalf"

![screenshot](/Images/17.jfif)

3. find all movies that have a synopsis that contains the word "Bilbo" and not the word "Gandalf"

![screenshot](/Images/18.jfif)

4. find all movies that have a synopsis that contains the word "dwarves" or "hobbit"

![screenshot](/Images/19.jfif)

5. find all movies that have a synopsis that contains the word "gold" and "dragon"

![screenshot](/Images/20.jfif)

- Delete Documents

1. delete the movie "Pee Wee Herman's Big Adventure"

![screenshot](/Images/21.jfif)

2. delete the movie "Avatar"

![screenshot](/Images/22.jfif)

## Relationships
  
- Insert the following documents into a `users` collection

username : GoodGuyGreg
first_name : "Good Guy"
last_name : "Greg"

![screenshot](/Images/23.jfif)

username : ScumbagSteve
full_name :
  first : "Scumbag"
  last : "Steve

![screenshot](/Images/24.jfif)

- Insert the following documents into a `posts` collection

username : GoodGuyGreg
title : Passes out at party
body : Wakes up early and cleans house

![screenshot](/Images/25.jfif)

username : GoodGuyGreg
title : Steals your identity
body : Raises your credit score

![screenshot](/Images/26.jfif)

username : GoodGuyGreg
title : Reports a bug in your code
body : Sends you a Pull Request

![screenshot](/Images/27.jfif)

username : ScumbagSteve
title : Borrows something
body : Sells it

![screenshot](/Images/28.jfif)

username : ScumbagSteve
title : Borrows everything
body : The end

![screenshot](/Images/29.jfif)

username : ScumbagSteve
title : Forks your repo on github
body : Sets to private

![screenshot](/Images/30.jfif)

- Insert the following documents into a `comments` collection

username : GoodGuyGreg
comment : Hope you got a good deal!
post : [post_obj_id]

![screenshot](/Images/31.jfif)

username : GoodGuyGreg
comment : What's mine is yours!
post : [post_obj_id]

![screenshot](/Images/32.jfif)

username : GoodGuyGreg
comment : Don't violate the licensing agreement!
post : [post_obj_id]

![screenshot](/Images/33.jfif)

username : ScumbagSteve
comment : It still isn't clean
post : [post_obj_id]

![screenshot](/Images/34.jfif)

username : ScumbagSteve
comment : Denied your PR cause I found a hack
post : [post_obj_id]

![screenshot](/Images/35.jfif)

- Querying related collections

1. Find all users

![screenshot](/Images/36.jfif)

2. Find all posts

![screenshot](/Images/37.jfif)

3. Find all posts that was authored by "GoodGuyGreg"

![screenshot](/Images/38.jfif)

4. Find all posts that was authored by "ScumbagSteve"

![screenshot](/Images/39.jfif)

5. Find all comments

![screenshot](/Images/40.jfif)

6. Find all comments that was authored by "GoodGuyGreg"

![screenshot](/Images/41.jfif)

7. Find all comments that was authored by "ScumbagSteve"

![screenshot](/Images/42.jfif)

8. Find all comments belonging to the post "Reports a bug in your code"

![screenshot](/Images/43.jfif)
