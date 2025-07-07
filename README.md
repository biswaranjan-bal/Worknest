Worknest: Freelance Connect

Worknest is a freelance marketplace web application built with the MERN stack (MongoDB, Express.js, React, Node.js). It connects freelancers and clients, allowing them to collaborate on projects, post job listings, and manage work efficiently.

📁 Project Structure

worknest-freelance-connect/
│
├── backend/ # Express.js backend with MongoDB
│ ├── models/
│ ├── routes/
│ ├── controllers/
│ ├── .env.example
│ ├── server.js
│ └── ...
│
├── frontend/ # React.js frontend
│ ├── public/
│ ├── src/
│ ├── .env.example
│ ├── package.json
│ └── ...
│
└── README.md


Features

User authentication and authorization (JWT)
Freelancer and client profiles
Job postings and applications
Messaging system
Responsive UI
Dashboard for users to manage projects

🛠️ Tech Stack

Frontend: React, Redux (Tailwind CSS / Bootstrap)
Backend: Node.js, Express.js, MongoDB, Mongoose
Authentication: JWT
Database: MongoDB 

⚙️ Installation & Setup

1] Install Node.js version 20 or above along with the package manager and MongoDB.

2] Must have a code editor like VScode as it allows you to access multiple shell entries simultaneously.

3] Open Main Project folder on VScode.

4] Run the following in both the "frontend" and "backend" folders:
             ~bash
              npm install (it updates and installs all dependencies required, and even the environment variables)
   If the terminal shows issue with bcrypt then forcefully install the audit fix: npm audit fix/ npm audit fix force

5] Start MongoDB and set up the following ENV files: 

Backend:

`JWT_SECRET`
e.g. this_is_secret_123

`MONGODB_URI`
e.g. mongodb cluster URI that need to be copied from the Connection Established that is known as the connection string there.

`SMTP`
e.g. Secret key establishment, there's a slight minor setup required here, install nodemailer in the bash and then 
If you're using Gmail(the otp will be sent from this mail to the authenticator) , you need to allow secure access:

Use an App Password:

Go to: https://myaccount.google.com/security
Turn on 2-Step Verification
Go to App Passwords → generate a password for "Mail"
Use that app password in the code
Use this mail as the 'STMP_MAIL' in the .env file


`NODE_ENV`
e.g. 'development' for local and 'production' for production

`DEV_CORS_ORIGIN`
e.g. http://localhost:8080 (client localhost)

`PROD_CORS_ORIGIN`
e.g. client deployed link (https://yourProjectName.com) 

Frontend

`CREATE_API_URL`
e.g. http://localhost:3000/api or production deployed server link


6) Run following in both "client" and "server" folders:
bash
npm start
 

