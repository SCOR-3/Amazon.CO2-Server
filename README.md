# Amazon.CO2-Server

This project serves as a very slim backend designed to work with Amazon.CO2 on Demand's sample [website](https://heroic-valkyrie-d7ef27.netlify.app/). This server receives purchase requests issued by the sample applications, and forwards these requests to Amazon.CO2 client site.

The server itself is implemented in [nodeJS](https://nodejs.org/en/about). Even if you are not familiar with the language do not worry, as the code has been extensively documented. The deployed backend server can be accessed using this [link](https://graceful-foal-hose.cyclic.app).

### One of the contributors deployed the server from his personal account. This allows [access](https://github.com/chinmayagarwal03/Amazon.CO2-Server) to the original repository.

The server logs all API requests it performs to the terminal, so you can see what's going on even without diving into the code.

## Integration with the Amazon.CO2 on Demand API
This sample backend interacts directly with Amazon.CO2's on Demand API, specifically for the purpose of authorizing and capturing orders. You can read more about the API [here](https://documenter.getpostman.com/view/21719363/2s9YRCVAPa#7c92258f-98d2-4b20-a60a-1265bc639134).

## Running the server
If you wish to run the server, the first step is [installing Node](https://nodejs.org/en/download).
Once that's out of the way, open a terminal and run the following command:

```
npm init
```
```
npm install
```

These commands would install the project's dependencies. 


The server is now ready to run. Simply point a terminal to the project's folder and run:

```
npm start
```

Alternatively you can run the following command 
```
nodemon start
```

### Using your credentials
The server's code includes MONGO_URL and JWT_SECRET which you have to set up for successfully running the server. You can use your own credentials by setting the `MONGO_URL` and `JWT_SECRET` environment variables before running the server. 
