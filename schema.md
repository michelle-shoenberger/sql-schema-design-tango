#Visualize your schema

Open this file in your text editor and visualize your schema. At the top is your table name. Listed below are all the columns in that table. 

User
-------------------
id
first_name
last_name

Address
-------------------
id
user_id
street 
street2 
city
state
zip_code
country

In the example above, each Address can belong to a User. This is achieved by adding a column called `user_id`, which can match only ONE of the values in the `id` column of the User table. Remember, `id`s are unique; no table can have two `id` values that are the same.

Using the above format, jot down the database for your apps below!

## GrubHub Online Ordering
Users
-------------------
id
first_name
last_name
address

Restaurants
-------------------
id
name
address

Menus
-------------------
id
restaurant_id
menu-item_id

Menu-items
-------------------
id
name
price

Orders
-------------------
user_id
menu-item_id
restaurant_id

## Blue Apron

Users
-------------------
id
first_name
last_name
address
service-plan_id

Service-Plans
-------------------
id
name
price

Menus
-------------------
id
service-plan_id
recipe_id

Recipes
-------------------
id
name
time

## Instagram

Users
-------------------
id
first_name
last_name
address

Posts
-------------------
id 
user_id
text
date

Comments
------------------
id
user_id
date
post_id
text

Likes
-------------------
id
user_id
post_id

Follows
-------------------
id 
user_id (followee)
user_id (follower)