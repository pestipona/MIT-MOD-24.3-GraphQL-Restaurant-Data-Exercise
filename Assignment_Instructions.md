# Module 24.3 - GraphQL Restaurant Data Exercise:

![GraphQL_Restaurant_Data_Exercise_01.png](Screen_Shots%2FGraphQL_Restaurant_Data_Exercise_01.png)

## Learning Outcome Addressed:

9. Use GraphQL to query and update data

Creating **multi-tier applications** means building **multiple API endpoints** to handle **different data operations**. The **more complex** your **application becomes**, *the harder it is to* **maintain all these endpoints**. `GraphQL` aims to **reduce this complexity** by providing a **simpler view** of **data** and making it **easier to query** it.

Your task is to **set up** `GraphQL` for your **restaurant data** and then **add mutations** to **get** and **update these data**.

The [starter files](/Starter_Files) for this activity include the **restaurant data** in **JSON format** and a predefined **build schema** for `GraphQL`. You need to **go through this code** to understand **what each query** or **mutation** should **look like**.

To **accomplish this task**, you **need to implement** the **following methods** under the `“root”` object:

* **restaurant:** This *gets* a *single restaurant* based on a *provided ID*.
* **restaurants:** This *gets* a *list of all* restaurants.
* **setrestaurant:** This *creates* a *new restaurant*.
* **Deleterestaurant:** This *deletes a restaurant* based on the *provided id*.
* **editrestaurant:** This *updates* a *restaurant* based on the *provided id*.

## Instructions:

After **completing the task**, run the **GraphQL interface** and **submit a file** with **screenshots** showing all **five queries** and **mutations** highlighted above, along with **a link** to your **GitHub repo** that **houses the code** for **this activity**.

## Solution:

First **let's setup** our **GraphQL environment**.

```shell
cd "D:\My Documents\MIT Full Stack Development\Module 24 - Express And GraphQL\Module 24.0 - Express And GraphQL\Self-Study_Activities\24.2.17 GraphQL Tool Update-Delete Exercise"

mkdir expressGraphQL01
cd expressGraphQL01
npm init
npm install express express-graphql graphql --save
```

![GraphQL_Restaurant_Data_Exercise_04.png](Screen_Shots%2FGraphQL_Restaurant_Data_Exercise_04.png)

![GraphQL_Restaurant_Data_Exercise_05.png](Screen_Shots%2FGraphQL_Restaurant_Data_Exercise_05.png)

Next, Let's import `index.js` and bring up a **terminal window** and let's do `node index.js`.

```shell
nodemon index.js
```