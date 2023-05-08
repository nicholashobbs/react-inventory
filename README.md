1. First, make sure you have Node.js and NPM (Node Package Manager) installed on your machine. You can download and install them from the official Node.js website: https://nodejs.org/en/download/

2. Once you have Node.js and NPM installed, you can create a new React app using the `create-react-app` command. Open a terminal and run the following command:

```
npx create-react-app my-app
```

Replace `my-app` with the name of your app. This command will create a new React app in a directory named `my-app`.

3. Next, you need to install the dependencies for connecting to Postgres. In the terminal, navigate to the root directory of your React app and run the following command:

```
npm install pg
```

This command will install the `pg` package, which is a PostgreSQL client for Node.js.

4. After installing the `pg` package, you need to create a new database in Postgres for your app to use. Open a terminal and run the following command:

```
createdb my_database
```

Replace `my_database` with the name of your database. This command will create a new database in Postgres with the specified name.

5. Finally, you need to set up the connection to the Postgres database in your React app. In the root directory of your app, create a new file called `.env.local` and add the following line:

```
DATABASE_URL=postgres://localhost:5432/my_database
```

Replace `my_database` with the name of your database. This line tells your app to connect to the database at `localhost:5432` (the default location for a locally hosted Postgres database) using the `my_database` database.

That's it for the first few steps! In the next steps, we will create a Node.js server to handle database connections and API requests from our React app.