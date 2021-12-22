Objective of this Test:
- Create a category "Special Items" and add an item "Special Item" to that category.
- When hovering over an item, show the items second image.
- Add a button that adds all items from the category to the shopping cart.
- If there are items in the cart, create another button which removes all items from the cart.
- Show an alert/notification to the user that the buttons have succeeded/failed.

My Solutions:

- Creating the item and category were fairly simple, done in bigcommerce admin page.

- As for the images on the item, a simple onmouseover and onmouseout were implemented to switch between the images src from the given array theme object.

- When implementing the "Add all items" button, with handlebars syntax I retrieved the category products and product ID's. With this I was able to pass them into an onClick function that fetched the Storefront API, adding the array of items into the cart by id.

- When implementing the "Remove all items", similarly, I grabbed the Cart ID given by the theme object using handlebars syntax. Passing that down into the onClick function, where I fetched the Storefront API to delete the cart entirely by its ID.

- And finally, once the promise returns, if successful I'd insert the success message into a div, vice versa, it would return an error message if an error was caught.


My Bigcommerce Store : https://fernandos-store.mybigcommerce.com/
Preview Code : c78d4svdth
