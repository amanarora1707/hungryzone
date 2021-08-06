![logo](https://user-images.githubusercontent.com/66989611/122261730-5053aa80-cef2-11eb-8f19-2d533f8119ab.png)


- It is a **food order app** deployed on [https://hungryzone-aman.herokuapp.com](url)

- I  made this app using **HTML, Tailwind CSS,JS,Node.js,Express.js,MongoDB,Socket.IO,Passport.js**

- You can order food with **real-time order tracking** as the store admin can update the order status using his login id.

<br>

 

- <h3>Welcome  Page </h3>

![Screenshot (28)](https://user-images.githubusercontent.com/66989611/122246229-006de700-cee4-11eb-8df5-0c5ebc5b6be3.png)

- When a customer comes to our app a **new session** is created that remain valid for **24hrs** which means if the user adds items to the cart without logging in and comes back after some time or cancel the tab for clearing tabs then using cookies in the browser the cart of the person will be there. So our esteemed customers should not worry about selected cart items.

<br>







- <h3> Menu </h3>

![Screenshot (33)](https://user-images.githubusercontent.com/66989611/122246657-5cd10680-cee4-11eb-91f2-f128db9c4d16.png)

- You can select from a wide range of food items and a **notification pops up** when we add any item to the cart. Menu items are saved in BSON format in non-sql database **MongoDB** . You can see the menu in  menus.json file in the repository where each item in the menu is linked with a unique id.


<br>

- <h3>Cart</h3>

![Screenshot (34)](https://user-images.githubusercontent.com/66989611/122246794-7c682f00-cee4-11eb-9563-e509408da936.png)

You can add items in cart but you cannot place order if you are not logged in. So if you want to order food you can simply login and if you are a new customer you can register with us. Authentication here is managed by passport-local.It is a Passport strategy for authenticating with a username and password.This module lets us authenticate using a username and password.

<br>

- <h3> Login Page </h3>

![Screenshot (36)](https://user-images.githubusercontent.com/66989611/122268295-847e9980-cef9-11eb-8ced-667631d5ac13.png)

Simply u can log in with registered mail id and password and then you will be redirected to your orders page.

<br>



- <h3>Playing with links </h3>

![Screenshot (40)](https://user-images.githubusercontent.com/66989611/122269172-8b59dc00-cefa-11eb-818b-b1d1a7822e4a.png)

It is possible that some users can try to come up with new ideas of manipulating links in their order id in all such cases users will be redirected 404 error page and if the customer is logged in then the customer will be redirected to welcome page/home page.

<br>

- <h3> Tracking Order </h3>
![Screenshot (39)](https://user-images.githubusercontent.com/66989611/122280137-800cad80-cf06-11eb-8972-00e720429b00.png)

- Realtime order tracking is done using socket.io
