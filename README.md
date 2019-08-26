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

#### GET /api/

Server returns:


[
      {
        restaurant_name: "Pizza Hut",
        restaurant_type: "Italian-American cuisine",
        user_id: 1,
        menu_id: 1
      } , {
        restaurant_name: "Burger King",
        restaurant_type: "Fast Food",
        user_id: 2,
        menu_id: 2
      },  {
        restaurant_name: "Mcdonalds",
        restaurant_type: "Fast-Food",
        user_id: 3,
        menu_id: 3
      },  {
        restaurant_name: "olive garden",
        restaurant_type: "Italian cuisine",
        user_id: 4,
        menu_id: 4
      } , {
        restaurant_name: "Chili's Grill & Bar ",
        restaurant_type: "American cuisine",
        user_id: 5,
        menu_id: 5
      },  {
        restaurant_name: " Buffalo Wild Wings",
        restaurant_type: "American cuisine",
        user_id: 6,
        menu_id: 6
      }
    ]


#### POST /api/ ##

User can post


{
   "restaurant_name":"name",
"restaurant_type":"type",
"user_id":req.params.id,
"menu_id":req.params.id
}

#### DELETE /api/:id

delete by id



### PUT  /api/:id

User can edit


{
"restaurant_name":"name",
"restaurant_type":"type",
"user_id":req.params.id,
"menu_id":req.params.id
}

####first react senior done ###

####################################
####################################

####################################
####################################

### Displays list of menu items

#### GET /api/menu

#### second react senior

Server returns:


[
      {
        item_name: "pizza",

        photo_of_order:
          "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png",
        review_id: 1,
        food_rating: 3.0
      },  {
        item_name: "Whopper",

        photo_of_order:
          "https://www.stickpng.com/assets/images/5882488ae81acb96424ffaaf.png",
        review_id: 2,
        food_rating: 4.0
      },
      {
        item_name: "Big Mac",

        photo_of_order:
          "https://i.redd.it/bydegsnwwhp11.png",
        review_id: 3,
        food_rating: 4.5
      },  {
        item_name: "spaghetti and meatballs",

        photo_of_order:
          "https://www.pastapass.com/images/dish1.png",
        review_id: 4,
        food_rating: 5.0
      }, {
        item_name: "Chicken steak fish and chips",

        photo_of_order:
          "https://www.pngkey.com/png/detail/21-216126_chicken-steak-fish-and-chips.png",
        review_id: 5,
        food_rating: 5.0
      },  {
        item_name: "BBQ hot wings",

        photo_of_order:
          "http://www.pngmart.com/files/8/Grilled-Food-PNG-Clipart-Background.png",
        review_id: 6,
        food_rating: 4.0
      }
    ]


---

#### POST /api/menu

User can post


{

 "menu_item_name":"name",
"restaurant_type":"type",
"photo_of_order":photo url,
"food_rating": a number,
"review_id":req.params.id

}

#### DELETE /api/menu/:id

delete by id



### PUT  /api/menu:id

User can edit


{
"menu_item_name":"name",
"restaurant_type":"type",
"photo_of_order":photo url,
"food_rating": a number,
review_id:req.params.id
}

#### second react done

####################################
####################################

####################################
####################################

### Displays list of menu items

#### GET /api/menu

#### third react senior

Server returns:


[
      {
        comments: "this is a great place to eat",
        price: 7.45,
        wait_time: "30min",
        date_of_visit: "01/30/2019",
        menu_id: 1
      }, {
        comments: "fast fun service",
        price: 8.74,
        wait_time: "10min",
        date_of_visit: "02/05/2019",
        menu_id: 2
      }, {
        comments: "i order with no pickles and received pickles i will not be returning",
        price: 8.00,
        wait_time: "9min",
        date_of_visit: "03/10/2019",
        menu_id: 3
      },  {
        comments: "my favorite go to spot ",
        price: 12.10,
        wait_time: "40min",
        date_of_visit: "05/27/2019",
        menu_id: 4
      }, {
        comments: "the right amount of spice and the right amount of alcohol i <3 this place",
        price: 13.24,
        wait_time: "45min",
        date_of_visit: "04/09/2019",
        menu_id: 5
      }, {
        comments: "mm i had better wings",
        price: 15.00,
        wait_time: "40min",
        date_of_visit: "01/30/2019",
        menu_id: 6
      }
    ]


---

#### POST /api/menu

User can post


{
   "comments":"put a comment",
"price":"a decimal",
"wait_time":a string,
"date_of_visit": "a string",
menu_id:req.params.id
}

#### DELETE /api/menu/:id  #####

delete by id



### PUT  /api/menu:id ######

User can edit


{
"comments":"put a comment",
"price":"a decimal",
"wait_time":a string,
"date_of_visit": "a string",
menu_id:req.params.id
}

#### third react done

######

####################################
####################################

####################################
####################################

####################################
####################################

####################################
####################################

###########react junior devs #################

#### GET /detail

#### first react junior dev

Server returns:


[
{
"id": 1,
"item_name": "pizza",
"photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png"
},
{
"id": 2,
"item_name": "Whopper",
"photo_of_order": "https://www.stickpng.com/assets/images/5882488ae81acb96424ffaaf.png"
},
{
"id": 3,
"item_name": "Big Mac",
"photo_of_order": "https://i.redd.it/bydegsnwwhp11.png"
},
{
"id": 4,
"item_name": "spaghetti and meatballs",
"photo_of_order": "https://www.pastapass.com/images/dish1.png"
},
{
"id": 5,
"item_name": "Chicken steak fish and chips",
"photo_of_order": "https://www.pngkey.com/png/detail/21-216126_chicken-steak-fish-and-chips.png"
},
{
"id": 6,
"item_name": "BBQ hot wings",
"photo_of_order": "http://www.pngmart.com/files/8/Grilled-Food-PNG-Clipart-Background.png"
}
]


---

#### GET /detail/:id

### more detail on the item name

Server returns:

[
{
"id": 1,
"comments": "this is a great place to eat",
"price": 7.45,
"item_name": "pizza",
"food_rating": 3,
"wait_time": "30min",
"date_of_visit": "01/30/2019",
"photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png"
}
]

#### first react junior dev done

#### GET /public

#### second react junior dev

Server returns:


[
{
"id": 1,
"restaurant_name": "Pizza Hut",
"restaurant_type": "Italian-American cuisine"
},
{
"id": 2,
"restaurant_name": "Burger King",
"restaurant_type": "Fast Food"
},
{
"id": 3,
"restaurant_name": "Mcdonalds",
"restaurant_type": "Fast-Food"
},
{
"id": 4,
"restaurant_name": "olive garden",
"restaurant_type": "Italian cuisine"
},
{
"id": 5,
"restaurant_name": "Chili's Grill & Bar ",
"restaurant_type": "American cuisine"
},
{
"id": 6,
"restaurant_name": " Buffalo Wild Wings",
"restaurant_type": "American cuisine"
}
]


---

#### GET /public/:id

### more detail on the item name

Server returns:

[
{
"id": 1,
"restaurant_name": "Pizza Hut",
"restaurant_type": "Italian-American cuisine",
"item_name": "pizza",
"food_rating": 3,
"photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png"
}
]

#### GET /public/detail/:id

### more detail on the item name

Server returns:

[
{
"id": 1,
"comments": "this is a great place to eat",
"price": 7.45,
"item_name": "pizza",
"food_rating": 3,
"wait_time": "30min",
"date_of_visit": "01/30/2019",
"photo_of_order": "https://www.pngfind.com/pngs/m/327-3272002_free-png-pizza-png-png-image-with-transparent.png"
}
]

#### second react junior dev done
