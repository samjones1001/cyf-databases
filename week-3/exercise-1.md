# Exercise 1


### Setup

- Clone the repository at https://github.com/samjones1001/cyf_hotels_api/blob/stage-one/server.js
- cd into the newly created directory with `cd cyf_hotels_api`
- switch to the `stage-1` branch with `git checkout stage-1`
- run the application with `node server.js`

### Testing the routes

- Open your browser and navigate to `http://localhost:3001/hotels`
- Navigate to `http://localhost:3001/hotel/1`
- Try adding different ids to the end of the above url. What will happen if you add an id which does not exist in your hotels table?

### Questions to consider

Imagine you had built a react frontend to communicate with this api. Think about the flow of data from the user, down to the database and back again.

BROWSER -> REACT -> HTTP -> SERVER -> MONGODB -> SERVER -> HTTP -> REACT -> BROWSER

You can use any method you like to describe each stage: it could be a diagram, flow chart or code snippets if you prefer.
Think about the following:
- How does data get sent between the server and the client?
- How does the Node server communicate with PostreSQL?
- What format does the data get transferred in?
- How does React display this data?
