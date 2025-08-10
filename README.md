
## C : CUSTOMIZE THE HTML
Customize the HTML user interface for your customer’s application. The user interface should include the shop name, the product names, and the names of the parts.
1. changes: changed name of site, changed haeders to match.
2. prompts : html
3. file name: mainscreen.html
4. line numbers: 14,19,21
5. dante of change: 10/10/24

Note: Do not remove any elements that were included in the screen. You may add any additional elements you would like or any images, colors, and styles, although it is not required.

## D : ADD AN ABOUT PAGE
Add an “About” page to the application to describe your chosen customer’s company to web viewers and include navigation to and from the “About” page and the main screen.
1. changes: made about html, made controller about us and added button on main screen
2. prompts : html , controller 
3. file name: about.html , AboutUsController, mainscreen.html
4. line numbers: about html lines 15-22, controller about us - lines 7-16, mains screen html line 17 
5. dante of change: 10/10/24

## E : ADD SAMPLE INVENTORY
Add a sample inventory appropriate for your chosen store to the application. You should have five parts and five products in your sample inventory and should not overwrite existing data in the database.
1. changes: added inventory
2. prompts : java
3. file name: boostrapData
4. line numbers: boostrap : 47-129, 133-146
5. dante of change: 10/13/24

Note: Make sure the sample inventory is added only when both the part and product lists are empty. When adding the sample inventory appropriate for the store, the inventory is stored in a set so duplicate items cannot be added to your products. When duplicate items are added, make a “multi-pack” part.

## F : BUY NOW BUTTON
Add a “Buy Now” button to your product list. Your “Buy Now” button must meet each of the following parameters:
The “Buy Now” button must be next to the buttons that update and delete products.
The button should decrement the inventory of that product by one. It should not affect the inventory of any of the associated parts.
Display a message that indicates the success or failure of a purchase.
1. changes: buyProduct method that decreases if greater than 1, buy now button, success and fail pages
2. prompts : html, controller
3. file name: addproductController, mainscreen, confrimationBuyProduct, failedBuyProduct
4. line numbers: addProductController : line 177-190**, mainscreen: 85-94, confirmationBuyProduct: 8-11, failedBuyProduct: 8-11
5. dante of change: 10/13/24 ... **updated 10/17/24

## G : MAX AND MIN INVENTORY
Modify the parts to track maximum and minimum inventory by doing the following:
Add additional fields to the part entity for maximum and minimum inventory.
Modify the sample inventory to include the maximum and minimum fields.
Add to the InhousePartForm and OutsourcedPartForm forms additional text inputs for the inventory so the user can set the maximum and minimum values.
Rename the file the persistent storage is saved to.
Modify the code to enforce that the inventory is between or at the minimum and maximum value.
1. changes: made min and max, checks for min and max, changed database file
2. prompts : html, java, controller
3. file name: parts, inHouse html, outSourced html, applicationProperties, addInhouseParts, addOutsourcedParts
4. line numbers: outSourced html: 25-32, inHouse html: 25-33, part: 31-39, 118 -122, addInhouse : 42-46, addOutsourced: 43-47, applicationProperties: 7
5. dante of change: 10/13/24

## H : INVENTORY VALIDATIONS 
Add validation for between or at the maximum and minimum fields. The validation must include the following:
Display error messages for low inventory when adding and updating parts if the inventory is less than the minimum number of parts.
Display error messages for low inventory when adding and updating products lowers the part inventory below the minimum.
Display error messages when adding and updating parts if the inventory is greater than the maximum.
1. changes: more validations, checking validator
2. prompts : java, controller
3. file name: addInhousePart controller, addOutsourcedPart controller, EnufPartsValidator
4. line numbers: addInhouse : 42-55, addOutsourced: 42- 56, EnufPartsValidator: 37-48 
5. dante of change: 10/13/24

## I : UNIT TEST
Add at least two unit tests for the maximum and minimum fields to the PartTest class in the test package.
1. changes: added testing for min and max in the test file
2. prompts : java
3. file name: partTest
4. line numbers: 129-150
5. dante of change: 10/13/24

## J : REMOVE UNUSED VALIDATORS
Remove the class files for any unused validators in order to clean your code.
1. changes: deleted DeletePartValidator
2. prompts : deletion
3. file name: DeletePartValidator
4. line numbers: deleted file
5. dante of change: 10/13/24

## OTHER

B.  Create a README file that includes notes describing where in the code to find the changes you made for each of parts C to J. Each note should include the prompt, file name, line number, and change.
