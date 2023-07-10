# Expensy
* This is a Flutter application that tracks down all your expenses and gives you a net balance.
* You can also choose the category of your expense and see them easily in the form of a list with icons on the main page.
* The charts page shows the daily, monthly, weekly and yearly expenses in form of charts.
* The application uses Hive, which is a NoSQL database, to store the data and syncfusion_flutter_charts for plotting the graph.

## UI
<img src="https://github.com/manohar-iitg/Expensy/assets/96137651/3e8faa87-c212-4979-afd5-3d77fb1a820a" height=600, width=300>
<img src="https://github.com/manohar-iitg/Expensy/assets/96137651/8dcd2450-fc07-4478-99f1-6b274e9e8d18" height=600, width=300>
<img src="https://github.com/manohar-iitg/Expensy/assets/96137651/84eeb63c-2232-48a8-91b8-0c0b6fd4366c" height=600, width=300>

## Bottom Navigation Bar
The navigation bar has three icons -
* Home, which navigates to the hope page.
* Chart, which navigates to the statistics page.
* Add, which opens up page where we can enter new data.

## Home Page
* The home page fetches the data from the local Hive storage.
* It shows all the transactions in the form of a scrollable list where users can see the category, date of transaction and amount recieved/spent.
* It also shows the user, the net balance in his account by calculating income and expenses.

## Statistics Page
* The statistics page dispays the charts of spend analysis by fetching data from Hive.
* It has charts for amount spent hour wise in a day, day wise in a week, week wise in a month, month wise in an year.
* The charts only spline if the data is available and hence if the data for only two days is available, it plots that and the graph may feel a bit compressed than usual. This will be resolved in the further updates.

## Add Data Page
* The page has 5 entries to be made - Category, Description, Amount, Income/Expense, Date
* Category is a dropdown list which includes - Food, Entertainment, Transportation and Transfer.

## Future Plans
* Making a feature where on clicking on each ID, we get detailed information regarding the transaction.
* Giving category-wise spending analysis.
* Providing authentication feature with Firebase and storing the data online using Firestore instead of Hive.
