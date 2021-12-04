# How To Build Your First Discord.JS Discord Bot

Welcome to my guide! By the end of reading this, you should have a full Discord Bot coded and ready to go!
Follow these steps and you will be well on your way.

This setup will vary per Operating System and IDE chosen.

1. Install Node.js v16.8.0
   Start of by installing NVM. Please select the correct way to install per OS:
   - Windows: www.shorturl.at/ryGY4
   - Linux: www.shorturl.at/tuOPV
   - macOS: www.shorturl.at/jsC17

   Once the correct NVM has been installed for your operating system, do the following
   ```js
    nvm install v16.8.0```

2. Initialize your folder
   Run: 
   ```js
     npm init```
   
   
2.1.
   It does not really matter how you configure your Initialisation but when you reach `entry point` you will need to note of the file name (e.g index.js).

3. Install the required modules.
   
   Launch a terminal window, please make sure you are in the directory of the `npm init` folder you just did in step 2. 
   Then run the following:
   ```js
      npm i discord.js```

4. Create a file called `index.js`
  
   If this file already exists, skip this step.
   This is where we start the actual coding.
   Open the `index.js` in your preferred code editor. We recommend Visual Studio Code.

5. Write the code needed in `index.js`

   Let's start by writing the requirements needed by the node process.
   Write the follow code into your file:

   ![image](https://user-images.githubusercontent.com/79745507/144714568-8e98c388-9543-45b3-a436-b4af85f56476.png)

   Lets walk through what this code means.
   The 1st line is defining `Client` and `Collection` and where they belong to, hence this time it comes from `discord.js`.
   The 2nd line is starting a new Discord Client with maxiumum intents (32767). Intents is basically maxiumum permissions in your server.
   The 3rd line is importing/requiring `discord.js` and we can use this module with `discord` as its identifier. 
   The 4th line is importing/requiring `config.json`, we will come back to this later. 

6. Setting up for testing

   Let's add a `console.log()` so we can test if our bot is responding.
   Write the following line into your code underneath your Step 5 code.

   ![image](https://user-images.githubusercontent.com/79745507/144714641-b3466ab2-9911-4a10-88a3-89af46dcf2a5.png)

   After this head back to your terminal from earlier and run:
   ```js
      npm i -g nodemon```
   
