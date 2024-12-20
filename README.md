# Weather Management System

## Project Overview
This project implements a comprehensive Weather Management System using a MySQL database and Node.js. The system is designed to store, manage, and analyze weather-related data such as forecasts, alerts, and user information. It demonstrates CRUD operations, advanced SQL queries, and database optimization techniques through indexing, triggers, views, and stored procedures.

---

## Features

### Database Features
- **City Information**: Stores details about cities, including their geographical attributes.
- **Weather Data**:
  - Real-time updates (current weather).
  - Daily and hourly forecasts.
  - Historical weather records.
- **Alerts**:
  - Weather alerts with descriptions, actions, and affected areas.
  - Triggers for automated alert generation based on extreme conditions.
- **User Management**:
  - User preferences mapped to cities.
  - CRUD operations for user data.

---

## How to Run the Project

### Prerequisites
Before starting, ensure you have the following installed:
1. **Node.js**: Install the latest stable version from [Node.js Official Website](https://nodejs.org/).
2. **MySQL Database**: Install MySQL and set up a local or remote database instance.
3. **Git** (optional): To clone the repository.

### Steps to Set Up and Run the Project

#### 1. Clone the Repository
If you haven’t already, clone the project repository from GitHub:
```bash
git clone https://github.com/your-username/weather-management-system.git
```

#### 2. Navigate to the Project Directory
Change into the project folder:
```bash
cd weather-management-system
```

#### 3. Install Dependencies
Use `npm` to install the required Node.js packages:
```bash
npm install
```
This will install dependencies like:
- `mysql`: To connect to the MySQL database.
- `prompt-sync` and `readline-sync`: For interactive command-line inputs.

#### 4. Set Up the Database
1. Open your MySQL client (e.g., MySQL Workbench or command-line interface).
2. Create a new database:
   ```sql
   CREATE DATABASE weather_management;
   ```
3. Import the SQL schema and data:
   - Locate the provided SQL file (e.g., `schema.sql`).
   - Import it into the `weather_management` database using your MySQL client or command-line:
     ```bash
     mysql -u your-username -p weather_management < schema.sql
     ```

#### 5. Update Database Configuration
Edit the `CRUD.js` file to configure database connection settings:
```javascript
const db = mysql.createConnection({
  host: 'localhost',
  user: 'your-username',
  password: 'your-password',
  database: 'weather_management'
});
```
Replace `your-username` and `your-password` with your MySQL credentials.

#### 6. Run the Application
Start the application by running the following command:
```bash
node CRUD.js
```

#### 7. Perform Operations
Follow the command-line prompts to:
- **Create a User**: Add a new user to the database.
- **Read User Data**: Fetch details for a specific user.
- **Update User Data**: Modify existing user information.
- **Delete a User**: Remove a user from the database.

### Additional Notes
- Ensure the database server is running before starting the application.
- Use the CSV files in the `data/` folder to populate additional tables if needed.

---

## Visual Demonstrations

### Example CLI Interaction
![CLI Interaction](https://via.placeholder.com/600x300?text=CLI+Interaction+Screenshot)
_Illustration of CRUD operations performed through the command-line interface._

### Database Schema
![Database Schema](https://via.placeholder.com/600x400?text=Database+Schema)
_Visual representation of the database schema, showing table relationships._

### SQL Query Example
![SQL Query Execution](https://via.placeholder.com/600x300?text=SQL+Query+Execution)
_Output of an advanced SQL query demonstrating aggregated data._

### Video Demonstration
[![Watch the demo video](https://via.placeholder.com/600x300?text=Demo+Video+Placeholder)](https://www.youtube.com/watch?v=your-video-id)

Click the thumbnail above to watch a demo video showcasing the project's features and functionality!

---

## Key Achievements
- Automated alert generation using triggers.
- Efficient querying through indexing and views.
- Aggregated analytics with OLAP and window functions.
- CLI-based application for database interaction.

---

## Future Enhancements
- **Security**:
  - Hash passwords using `bcrypt`.
- **Frontend**:
  - Build a web-based interface with `Express.js` and a frontend framework.
- **Real-Time Updates**:
  - Integrate APIs for live weather data.
- **Performance**:
  - Implement materialized views for frequently accessed data.

---

## Contributing
Feel free to fork this repository and contribute to the project. Submit a pull request for any enhancements or bug fixes.

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact
For any queries or suggestions, please reach out:
- **Email**: your-email@example.com
- **GitHub**: [your-username](https://github.com/your-username)
