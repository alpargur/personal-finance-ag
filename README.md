# Personal Finance Anonyme Gesellschaft

Welcome to Personal Finance Anonyme Gesellschaft! 💸

This is a place where you can keep track of your expenses and distribute your income as you want to.

Design Principles:

- Keep it simple !
- Have an overall insight !
- Make finance easy !

There is an excel file template available which holds the necessary table structure for analysis:

| date | fixcosts | grocery | shopping | food | activity | others | expenses-total | income | essential-expenses | essential-funds | discretionary-expenses | discretionary-funds | investment-expenses | investment-funds | savings |
| ---- | -------- | ------- | -------- | ---- | -------- | ------ | -------------- | ------ | ------------------ | --------------- | ---------------------- | ------------------- | ------------------- | ---------------- | ------- |

Besides, the excel template also includes some cell formulas making it easy to calculate some other column values (_e.g._ total-expenses or discretionary-funds). More on that below.

## Columns Explanations

Followings are the attributes which you need to provide your own information:

- **date:** The entries are made monthly, but you can adjust the time interval as you wish.
- **fixcosts:** A total of your fix expenses (rent, subscriptions, gym membership etc.)
- **grocery:** Things you buy from grocery store.
- **shopping:** The material stuff you buy (apparel, devices, moka pot, books that you don't bother to open and read)
- **food:** When you are to lazy to cook and order a pizza.
- **activity:** This is a very wide spectrum. It could be a night out with friends, a spontaneous trip to Colombia, a birthday party for your kid.
- **others:** This where usually unexpected costs fall. Such as locksmith charge when you lock yourself outside or hospital expenses.
- **expenses-total:** Sum of all expenditures. It is calculated automtically.
- **income:** Enter your income for selected timewindow. If you have multiple income streams provide the total sum.

Rest of the columns are relevant for resource allocation. You don't need to provide them (except future-expenses). Excel calculates them automatically depending on [50 / 30 / 20 rule](https://www.investopedia.com/ask/answers/022916/what-502030-budget-rule.asp).

- **essential-expenses:** Cost we humans pay to survive: fixcosts + grocery + food
- **essential-funds:** 50% of your income.
- **discretionary-expenses:** Cost we pay to purchase a big a$$ truck or eat at fancy restaurant and leave hungry, i did also added **others**. Adjust column in the excel template file if you want to keep it separately: shopping + activity + others
- **disretionary-funds:** 30% of your income.
- **investment-expenses:** The amount you reserve for your savings or investments. Don't forget, you need to provide it :)
- **investment-funds:** 20% of your income.
- **savings:** 30% of your income. This attribute is just to give a sense of how much you ought to save. Not included in 50 / 30 / 20 rule.

Excel file is there to provide necessary data for further analysis and the visualization of data. But it also provides visual feedback by comparing expenses-total vs income:

- If expenses-total exceeds the income: <span style="color:red">cell color is red</span>.
- If expenses-total is equal to the income: <span style="color:green">cell color is green</span>.
- Else: <span style="color:blue">cell color is blue</span>.

Same logic implies for essentials- and discrentionaries-.

If you have decided to use the template file and came this far, don"t forget to rename the `input-template.xlsx` to `input.xlsx`.

## Prepare Development Environment

1. Clone repository
2. Go to root directory of repository on your terminal
3. Create a virtual environment: `virtualenv venv`
4. Activate virtual environemnt: `source venv/bin/activate`
5. Install packages: `pip install -r requirements.txt`
