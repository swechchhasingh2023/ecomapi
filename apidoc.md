http://localhost:9111/electronics

http://localhost:9111/smartphones

http://localhost:9111/appliances

http://localhost:9111/grooming

http://localhost:9111/kitchen


// http://localhost:9108/category
x-access-auth
12345678abcdef213

> Rest wrt to category (GET)
http://localhost:9108/products?productId=1

Details Of Category
http://localhost:9108/details/4

menu wrt category ID
http://localhost:9108/menu/1

//page4
> Details of menu selected (POST)
http://localhost:9108/menuDetails
body> {"id":[101,102,103]}


> Place Order (POST)

post> http://localhost:9108/placeOrder

{
        "orderId": 3,
        "name": "Swechchha Singh",
        "email": "swesingh@gmail.com",
        "address": "Hom 65",
        "phone": 8934645457,
        "cost": 712,
        "menuItem": [
            101,102,103
        ],
        "status": "On The Way"
}

//page
> List all orders(GET)
get> http://localhost:9108/orders
http://localhost:9108/orders?swesingh@gmail.com



>update order(PUT)
http://localhost:9108/updateOrder
> body
{
    "_id": "671364dd23d5f476d5cc29f0",
    "status": "Pending"
}

>Delete order (DELETE)
http://localhost:9108/deleteOrder
{
    "_id": "671364dd23d5f476d5cc29f0"
}