logo

Backend Tickitz - Arkademy
🧐 About
This is the repository Backend of the Bootcamp Arkademy task

User Endpoint
METHOD	API	REMARKS
POST	/v1/users	Input Data To Table Users
GET	/v1/users/:userId	Get Data By userID
GET	/v1/users	Get All Data User
GET	/v1/users?page=xx&limit=xx	Get Data With Pagination
PUT	/v1/users/:userId	Edit Data By userID
DELETE	/v1/users/:userId	Delete Data By userID
Ticket Endpoint
METHOD	API	REMARKS
POST	/v1/tickets	Input Data To Table Ticket
GET	/v1/tickets/details/movie/:userId&?movie=:movieId	Get Ticket By userID & movieID
GET	/v1/tickets/details/user/:userId	Get All Ticket By userID
GET	/v1/tickets/details/user/:userId?page=xx&limit=xx	Get Ticket By userID With Pagination
GET	/v1/tickets/:userId?name=:movieName	Get Ticket By userID With Spesific Movie Name
GET	/v1/tickets?ticketId:ticketId	Get Ticket By ticketId
PUT	/v1/tickets/:userId?ticketId=:ticketId	Edit Ticket By userID & ticketID
DELETE	/v1/tickets/:userId?ticketId=:ticketId	Delete Ticket By userID & ticketID
Other endpoints are still in the documentation process
💻 Installation
Follow the steps below

Clone this repo
git clone https://github.com/therevolt/BE-Ticktiz
cd BE-Ticktiz
Install module & Import Database
Install Module
npm install
Import Database
Import tickitz.sql To Your Databases
You Can Follow This Steps

Create env file
# ---------------------------------------
#               CONFIG DB
# ---------------------------------------
DB_HOST= #host database
DB_USER= #user database
DB_PASS= #pass database
DB_NAME= #database name

# ---------------------------------------
#            CONFIG GENERAL
# ---------------------------------------
PORT= #port app
HOST= #host/domain app
Detail CONFIG GENERAL

EXAMPLE URL	http://localhost:6000
PORT	6000
HOST	http://localhost
Done, You can run it in the way below
Developer Mode (with nodemon)
npm run dev
Production Mode (only node)
npm start
🔖 Standard Response & Preview Request By Postman
Standard Response API
{
    "status": true,
    "message": "success register",
    "data": [object Object]
}
Object data contains content according to the request

Preview Request By Postman
Preview

⛏️ Built Using
ExpressJS
MySQL2 Package
CORS Package
Morgan Package
DotEnv Package
Redis Package
JWT Package
Nodemailer Package
UUID Package
Multer Package
Bcrypt Package
💭 Documentation
Click Here

💻 FrontEnd
Repo Frontend : https://github.com/therevolt/ReactJS-FE-Tickitz

💻 Live Demo
Netlify

✍️ Authors
@therevolt
