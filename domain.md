
1.
As a member of the public,
So I can order a bagel before work,
I'd like to add a specific type of bagel to my basket.

2.
As a member of the public,
So I can change my order,
I'd like to remove a bagel from my basket.

3.
As a member of the public,
So that I can not overfill my small bagel basket
I'd like to know when my basket is full when I try adding an item beyond my basket capacity.

4.
As a Bob's Bagels manager,
So that I can expand my business,
I�d like to change the capacity of baskets.

5.
As a member of the public
So that I can maintain my sanity
I'd like to know if I try to remove an item that doesn't exist in my basket.


| Classes    | Members                                      | Methods                                     | Scenario                                  | Outputs             |
|------------|----------------------------------------------|---------------------------------------------|-------------------------------------------|---------------------|
| `Basket`   | `List<Bagel> BagelList`                      | `AddBagel(Bagel bagel)`                     | Bagel is successfull added                | true                |
|            |                                              |                                             | Bagel is not added, basket full           | false               |
|            |                                              | `RemoveBagel(Bagel bagel)`                  | Bagel is Removed                          | true                |
|            |                                              |							                  | Bagel is not found, not removed           | false               |
|            | `int BagelCapacity`                          | `UpdatedCapacity(int newCap)`               |									          |                     |

6.
As a customer,
So I know how much money I need,
I'd like to know the total cost of items in my basket.

7.
As a customer,
So I know what the damage will be,
I'd like to know the cost of a bagel before I add it to my basket.

8.
As a customer,
So I can shake things up a bit,
I'd like to be able to choose fillings for my bagel.

9.
As a customer,
So I don't over-spend,
I'd like to know the cost of each filling before I add it to my bagel order.

10.
As the manager,
So we don't get any weird requests,
I want customers to only be able to order things that we stock in our inventory.


| Classes    | Members                                            | Methods                                     | Scenario                                  | Outputs             |
|------------|----------------------------------------------------|---------------------------------------------|-------------------------------------------|---------------------|
| `Basket`   | `List<Bagel> BagelList` & `List<Coffee> CoffeeList`| `GetTotalBasketSum()`                       |							                | decimal             |
|            |                                                    |                                             |								            |                     |
| `Inventory`| `List<(string, double, string, string)>`           | `CheckBagelPrice(string, name, varient)`    |                                           | decimal             |
|            |                                                    |	`CheckFillingPrice(string filling)`         |                                           | decimal             |
|            |													  |                                             |									        |                     |


11.
As a customer,
So that i get a discount,
I will buy 12 plain bagels for 3.99