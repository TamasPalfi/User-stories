<center><h1><b>Non-Functional Requirements</b></h1></center>

### FrontEnd 
***React.js***   
- React is very a simple and lightweight library that only deals with the view layer. It is not a beast like other MV* frameworks such as Angular or Ember. Since, one team is going to take care of the frontend, it's good for them to only focus on view layer using React.js 

- React provides a component based structure. As a result:
    - your app has consistent look and feel.
    - code re-use makes it easier to maintain and grow your codebase.
    - it is easier to develop your app.

- Updating DOM is usually the bottleneck when it comes to the web performance. React efficiently compares the previous and current states of the virtual DOM and calculates the best way (minimum amount of updates needed) to apply these changes. This is the main reason behind React’s high performance.


### Backend 
***Node.js***

- Since we already decided to use JavaScript(React.js) for frontend, it’s a no-brainer to pick Node.js(Javascript).

- Node.js use V8 engines by Google. Fast and scalable web apps in a result.

- Thanks to this popularity, a vicious cycle is set up: your favorite API might only offer an official Node.js library, and other languages are not even considered, left for unofficial packages 


### Credit Card Software 
***Stripe.js*** 
- In keeping with their principle of simplicity and convenience, pricing is 2.9% + $.30 per successful transaction.

-  There are extremely readable documentations and code samples to do efficient custom integration. 

- If developers want to test the application before making it live, they simply hit the “test” button. In comparison, PayPal makes developers set up a sandbox account and log in and out of different vendor and seller accounts.

### Automated Email 
***Sendgrid***

- Deliverability. : Avoids emails going to spam folder/rejection by mail server.  

- Easy integration with a dead simple API.

- Track email performance, reads, etc and verify whether emails have reached their destination and verifies whether email has reached destination. 

- Ability to prevent mailing to certain addresses in a separate layer, rather than relying on applications.

- By using this API, we can easily send invitation emails to new members and get a notification to the server when they accept it.

### Database 
***PostgreSQL***

- Postgres has a strongly typed schema that leaves very little room for errors. Developers first create the schema for a table and then add rows to the table. They can also define relationships between different tables with rules so that they can store related data across several tables and avoid data duplication

- Developers can put all the complex logic in a custom function, index it and the searches will be super fast. 

- PostgreSQL is an object-relational database, so arrays of values can be stored for most existing data types.

- Is not just relational but object-relational. Advantageous over other open source SQL databases such as MySQL, MariaDB and Firebird.

- Much more query features of SQL than MySQL.

***Our Preliminary Tables and their Associated Values***
- Member
    - email: string
    - password: string
    - isAdmin: boolean
    - points: integer
    - credit_card_number: integer
    - credit_card_cvv: integer
    - is_private: boolean

- Post
    - text: string
    - date_time: date and time field
    - user_key: key that links post to user

- Comments
    - text: string
    - date_time: date and time field
    - post_key: key to linked post
    - user_key: key to specific user

- Photos
    - photo: image file
    - user_key: key to associated user

- Filtered Photos
    - photo: image file
    - filter: tracks added content or filter
    - photo_key: key to original photo
    - user_key: key to associated user

### Application Map

![](done.jpg)
