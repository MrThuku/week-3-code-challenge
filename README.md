# Phase 3 Code Challenge: Product Reviews

## About the Application
This application uses Active Record to manage reviews of products. The application has three classes: User, Product, and Review. Each user can review multiple products, and each product can have multiple reviews. The Review class stores the star rating and comment for each review, as well as the user and product associated with the review.



 ## Classes and Methods
- Review
#### Instance Methods
#user: Returns the User instance for this Review
#product: Returns the Product instance for this Review
#print_review: Prints the details of the review in the terminal in the following format: "Review for {insert product name} by {insert user name}: {insert review star_rating}. {insert review comment}"
- Product
#### Instance Methods
#reviews: Returns a collection of all the Reviews for the Product
#users: Returns a collection of all the Users who reviewed the Product
#leave_review(user, star_rating, comment): Creates a new Review in the database associated with this Product and the User. Takes a User (an instance of the User class), a star_rating (integer), and a comment (string) as arguments.
#print_all_reviews: Prints the details of all the reviews for the product in the terminal. Each review is formatted in the same way as the #print_review method.
#average_rating: Returns a float representing the average star rating for all reviews for this product
- User
#### Instance Methods
#reviews: Returns a collection of all the Reviews that the User has given
#products: Returns a collection of all the Products that the User has reviewed
#favorite_product: Returns the product instance that has the highest star rating from this user
#remove_reviews(product): Removes all of this user's reviews for the given product. Takes a Product (an instance of the Product class) as an argument.
