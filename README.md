## Server

const PORT = process.env.PORT || 5000;
const io = require("socket.io")(PORT,

Deploy Heroku:
cd .\server
heroku login
git init
heroku git:remote -a react11-whatsapp-clone
git add .
git commit -am "first"
git push heroku master

Check deploy logs:
heroku logs --tail

--> https://heroku login.herokuapp.com/

## Client
  useEffect(() => {
    const newSocket = io(
      //'http://localhost:5000',
      'https://react11-whatsapp-clone.herokuapp.com',

npm run build

Deploy to Netlify

--> https://react11-whatsapp-clone.netlify.app/
