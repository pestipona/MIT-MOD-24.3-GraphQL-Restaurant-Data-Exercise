# Module 24.3 - GraphQL Restaurant Data Exercise:

![GraphQL_Restaurant_Data_Exercise_02.jpg](Screen_Shots%2FGraphQL_Restaurant_Data_Exercise_02.jpg)

## Project Description:

This multi-stack application demonstrates the use of GraphQL to efficiently perform query and mutation operations on a sample restaurant database. The query operations include getting a list of all the restaurants in the database, and getting a particular restaurant based on its id. The mutation operations involve editing an existing restaurant, deleting a restaurant from the database, and finally adding a new restaurant.

### Technical Stack:

* **Frontend:** The frontend `index.js` is developed using modern web technologies like React.js.

* **Backend:** The backend is powered by a `Node.js` server, which handles GraphQL requests and interactions with the restaurant database.

* **Database:** The database is hardcoded in the `index.js` file. For now this is a limitation. Since the application is for demonstration of concept only.

* **GraphQL Server:** The `GraphQL` server acts as a middleware that efficiently processes queries and mutations, communicating with the database to fetch or update the required information.

## Installation:

Click on the https url of the project repository and depending on which IDE you are using paste the URL in your git clone command in your terminal and within your project directory.

```shell
git clone <github url>
```

After successfully cloning the repository. Make sure you first have `Node.js` installed.

```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install node
node -v
npm -v
```

Then run the package.json file by running npm install to install all dependencies.

```shell
npm install
```

## Usage:

### Opening the Application:

In your IDE open up a terminal and navigate to the directory `expressGraphQL` and enter nodemon `index.js`

```shell
cd ./expressGraphQL
nodemon index.js
```

The application will **now start listening** on `port 5500`, open up a **web browser** go to http://localhost:5500/graphql. And if you get a `port 5500` and GraphQL, it actually means your environment is working.

![GraphQL_Restaurant_Data_Exercise_07.png](Screen_Shots%2FGraphQL_Restaurant_Data_Exercise_07.png)

### Return a list of all restaurants:

To perform a query in graphQL paste the following graphQL query called `restaurants` in the box as shown. This will return a list of all the restaurants.

```text
query restaurants{
  restaurants {
    id
		name
    description
    dishes {
      name
      price
    }
  }
}
```

As shown below:

![GraphQL_Restaurant_Data_Exercise_08.png](Screen_Shots%2FGraphQL_Restaurant_Data_Exercise_08.png)

## Future Improvements:

## License:

