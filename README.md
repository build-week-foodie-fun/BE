# BACK END [Foodie] => SUBJECT TO CHANGE

#### Back End Architect => Jason Aviles

---

## BASE URL:

#### https://buildweek-foodie1.herokuapp.com (she's alive!)

---

### admin sign up:

#### POST /auth/register

Client sends:


{
  "username": "new user name", //REQUIRED
  "password": "pass",          //REQUIRED
}


Server returns:


{
    "id": "5",
}


### admin log in (provides authentication token)

#### POST /auth/login

Client sends:


{
  "username": "new user name", //REQUIRED
  "password": "pass"           //REQUIRED

}


Server returns:


{
    "messsage": "Welcome username",
    "id": "5",
    "token": "big ol' hashed token"
}


---

#### auth routes for senior devs needs token#####################33

######################################################

### Displays list of restaurant

#### first react senior

#### GET /auth/api/

Server returns:


[
  {
    "id": 1,
    "restaurant_name": "Pizza Hut",
    "restaurant_type": "Italian-American cuisine",
    "created_at": "2019-08-26 20:20:07",
    "user_id": 1,
    "item_name": "pizza",
    "photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png",
    "food_rating": 3,
    "comments": "this is a great place to eat",
    "price": 7.45,
    "wait_time": "30min",
    "date_of_visit": "01/30/2019"
  },
  {
    "id": 2,
    "restaurant_name": "Burger King",
    "restaurant_type": "Fast Food",
    "created_at": "2019-08-26 20:20:07",
    "user_id": 2,
    "item_name": "Whopper",
    "photo_of_order": "https://www.stickpng.com/assets/images/5882488ae81acb96424ffaaf.png",
    "food_rating": 4,
    "comments": "fast fun service",
    "price": 8.74,
    "wait_time": "10min",
    "date_of_visit": "02/05/2019"
  },
  {
    "id": 3,
    "restaurant_name": "Mcdonalds",
    "restaurant_type": "Fast-Food",
    "created_at": "2019-08-26 20:20:07",
    "user_id": 3,
    "item_name": "Big Mac",
    "photo_of_order": "https://i.redd.it/bydegsnwwhp11.png",
    "food_rating": 4.5,
    "comments": "i order with no pickles and received pickles i will not be returning",
    "price": 8,
    "wait_time": "9min",
    "date_of_visit": "03/10/2019"
  },
  {
    "id": 4,
    "restaurant_name": "olive garden",
    "restaurant_type": "Italian cuisine",
    "created_at": "2019-08-26 20:20:07",
    "user_id": 4,
    "item_name": "spaghetti and meatballs",
    "photo_of_order": "https://www.pastapass.com/images/dish1.png",
    "food_rating": 5,
    "comments": "my favorite go to spot ",
    "price": 12.1,
    "wait_time": "40min",
    "date_of_visit": "05/27/2019"
  },
  {
    "id": 5,
    "restaurant_name": "Chili's Grill & Bar ",
    "restaurant_type": "American cuisine",
    "created_at": "2019-08-26 20:20:07",
    "user_id": 5,
    "item_name": "Chicken steak fish and chips",
    "photo_of_order": "https://www.pngkey.com/png/detail/21-216126_chicken-steak-fish-and-chips.png",
    "food_rating": 5,
    "comments": "the right amount of spice and the right amount of alcohol i <3 this place",
    "price": 13.24,
    "wait_time": "45min",
    "date_of_visit": "04/09/2019"
  },
  {
    "id": 6,
    "restaurant_name": " Buffalo Wild Wings",
    "restaurant_type": "American cuisine",
    "created_at": "2019-08-26 20:20:07",
    "user_id": 6,
    "item_name": "BBQ hot wings",
    "photo_of_order": "http://www.pngmart.com/files/8/Grilled-Food-PNG-Clipart-Background.png",
    "food_rating": 4,
    "comments": "mm i had better wings",
    "price": 15,
    "wait_time": "40min",
    "date_of_visit": "01/30/2019"
  }
]

#### POST /auth/api/ ##

User can post


{
  
  "restaurant_name": "Pizza Hut",
  "restaurant_type": "Italian-American cuisine",
  "user_id": 1,
  "item_name": "pizza",
  "photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png",
  "food_rating": 3,
  "comments": "this is a great place to eat",
  "price": 7.45,
  "wait_time": "30min",
  "date_of_visit": "01/30/2019"
}

#### DELETE /api/:id

delete by id



### PUT  /auth/api/:id

User can edit


{
"restaurant_name": "Pizza Hut",
  "restaurant_type": "Italian-American cuisine",
  "user_id": 1,
  "item_name": "pizza",
  "photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png",
  "food_rating": 3,
  "comments": "this is a great place to eat",
  "price": 7.45,
  "wait_time": "30min",
  "date_of_visit": "01/30/2019"
}



### GET BY ID  /auth/api/:id
{"restaurant_name": "Pizza Hut",
  "restaurant_type": "Italian-American cuisine",
  "user_id": 1,
  "item_name": "pizza",
  "photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png",
  "food_rating": 3,
  "comments": "this is a great place to eat",
  "price": 7.45,
  "wait_time": "30min",
  "date_of_visit": "01/30/2019"}

### GET USER /auth/api/users
gets all users





## public routes  /public

should get all reviews


## public routes by id  /public/:id


should get by a specific id


####first react senior done ###

####################################
####################################

####################################




