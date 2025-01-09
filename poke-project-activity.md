## Activity: Using PokeAPI with Different Methods

This activity will have you explore the PokeAPI and practice using different methods to fetch data: XMLHttpRequest, Fetch API with `.then()`, and Async/Await. 

**Preparation:**

1. **Clone the Repository:** 
    - You will need Git installed on your machine. 
    - Open a terminal window and navigate to your desired directory.
    - Run the command `git clone https://github.com/2164-ServiceNow/poke-project-htmlcssjs.git`. 
2. **Branch Selection:**
    - Navigate to the cloned directory using `cd poke-project-htmlcssjs`.
    - Checkout the `dev` branch using `git checkout dev`.
    - Choose a SINGLE user story (Optional Challenge: do both):
        - As a USER I can QUERY FOR ITEMS so that I CAN LEARN MORE ABOUT THEM
        - As a USER I can QUERY FOR MOVES so that I CAN LEARN HOW TO USE THEM

**Activity:**

1. **Create a Branch:**
    - ***Under the dev branch***, run the command `git checkout -b lastname-userstory` (replace `lastname-userstory` with your actual lastname and chosen user story).
2. **Explore PokeAPI:**
    - Visit the PokeAPI documentation to determine the endpoints you need for your asychronous requests: [https://pokeapi.co/](https://pokeapi.co/)
    - [Documentation for Moves](https://pokeapi.co/docs/v2#moves-section)
    - [Documentation for Items](https://pokeapi.co/docs/v2#items-section)

3. **Implement Data Fetching:**
- Look through the code in `queryPokemon.js` to obtain examples for each of the following forms of requesting information from an API.
- Generate a file for you user story that's named either `queryItems.js` or `queryMoves.js` to provided functionality.
- Add your new JavaScript file to the `index.html` with the script element
- Add a button to run your function from your JavaScript file you created.

    ### Implement below:
   1. **XMLHttpRequest:**
       - Generate a request using AJAX through the class `XMLHttpRequest` in JavaScript. See `queryPokemon.js`
       - Simply `console.log()` the information from the Response Body (JSON information)
       - **Afterwards you may comment out**
   2. **Fetch API with `.then()`:**
       - Create another function to fetch data using the Fetch API with the fetch-then-catch syntax as seen in `queryPokemon.js`
       - Simply `console.log()` the information from the Response Body (JSON information)
       - **Afterwards you may comment out**
   3. **Async/Await:**
       - Create yet another function for fetching data using Async/Await syntax as seen in `queryPokemon.js`
       - Simply `console.log()` the information from the Response Body (JSON information)
        - **Afterwards you may comment out**

**Update HTML for Website:**

- Choose either `fetch-then` or `async-await` based on your preference to execute the query action for yoru user story.
- Include HTML code to visualize the information through DOM Manipulation in `index.html`. Have fun with this, you can use anything from bootstrap, which has already been integrated with the project.
    - [Bootstrap docs](https://getbootstrap.com/docs/5.3/getting-started/introduction/)

**Commit, Push & Pull Request**
- Commit your code & push your branch to the remote repository
- Generate a pull request from `lastname-userstory` to `dev`. 
    - ***NOTE: DO NOT MERGE! Make sure you're not merging into `main` either, this can be fixed from the pull request as long as you DO NOT MERGE***

**Competition**
- Folks may volunteer their code to be reviewed live & voted for persistence in the codebase. 