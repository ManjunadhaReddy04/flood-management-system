# flood-management-system

About
The Flood Management System is a web-based application designed to assist coastal communities during flood emergencies. It leverages drones for efficient delivery of essential medicines and supplies to affected areas. Users can register on the platform, provide details about their medical conditions, required medications, and their location (e.g., house ID). Drones then deliver the necessary supplies directly to the specified locations, ensuring quick and reliable assistance even in isolated or hard-to-reach areas.

This system also includes an interactive dialpad feature, allowing users to request additional needs (e.g., water, more medicine) after receiving initial deliveries.

Features
User Registration : Coastal residents can register and provide their medical requirements and location details.
Drone Delivery : Drones deliver medicines and supplies directly to registered locations.
Interactive Dialpad : After receiving initial supplies, users can use a dialpad to request additional items in real time.
Map Interface : Administrators and users can track drone deliveries and view affected areas on a map.
Medication Tracking : Stores and manages user-specific medication data for accurate delivery.
Installation
Follow these steps to set up and run the application locally:

Prerequisites
Node.js (v20.17.0 or higher)
npm (v9.6.7 or higher)
PostgreSQL (v15.x or higher)

Steps :
1.Clone the Repository 
  bash-> git clone https://github.com/your-username/flood-management-system.git
2.Navigate to the Project Directory
  cd flood-management-system
3.Install Dependencies 
   npm install
4.Set Up the Database :
Create a PostgreSQL database named drpr.
Update the database credentials in index.js:
javascript
const db = new pg.Client({
  user: "postgres", // Replace with your PostgreSQL username
  host: "localhost",
  database: "drpr",
  password: "your_password", // Replace with your PostgreSQL password
  port: 5432,
});
5.Start the Application 
  npm start
  
Usage
Endpoints
Home Page : http://localhost:3000/
Register Page : http://localhost:3000/register
About Page : http://localhost:3000/about
Admin Map View : http://localhost:3000/admin
Logout : http://localhost:3000/logout
Submit Medication Data : POST /table
Update House ID : POST /update-house
Request Additional Needs : POST /update-need
Fetch Cold Houses : GET /get-cold-houses

How It Works
User Registration :
Navigate to the /register page and fill out the registration form with your details (e.g., username, password, disease, medication, etc.).
Upon successful registration, you’ll be redirected to the login page.
Login :
Use your registered credentials to log in from the home page (/).
Map Interface :
Once logged in, you’ll see a form fill and submit it and go to map section to select the your house. now you are all set . 
log out you and login as admin and start drone.
Use the dialpad to request additional needs (e.g., press 1 for water, 2 for more medicine).
Admin View :
Administrators can access the /admin route to view all registered users and manage deliveries.

screenshot :![Screenshot 2025-03-26 001327](https://github.com/user-attachments/assets/a6522aed-9fef-4b05-a834-cf7c7e659a96)

Contact
For questions or feedback, reach out to:

Email: manjupdrl025@gmail.com
LinkedIn:Venna Manjunadha reddy

Thank you


