ENVIRONMENT VARIABLE:
npm install dotenv --> used to define an environment variable such as the MONGODB_URI
create a .env file
--> e.g. MONGODB_URI='mongodb+srv://fullstack:sekred@cluster0-ostce.mongodb.net/note-app?retryWrites=true'
PORT=3001
add it in .gitignore

    add the following to index.js file
        require('dotenv').config()
        const Note = require('./models/note')
        const PORT = process.env.PORT
        FYI: dotenv gets to be imported before note model
