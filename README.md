 🏥 Hospital Management System

A full-stack **Hospital Management System** built using the **MERN Stack** (MongoDB Atlas, Express.js, React.js, Node.js). The application allows hospital staff to manage patient records through a simple and responsive interface with complete CRUD functionality.

---

## 📌 Features

- Add (Admit) a new patient
- View all admitted patients
- Update patient details
- Discharge (Delete) a patient
- Search patients by name or disease
- Responsive UI
- MongoDB Atlas database integration
- RESTful API
- Postman collection for API testing

---

## 🛠️ Tech Stack

### Frontend
- React.js
- CSS3
- Fetch API

### Backend
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- CORS

---

## 📂 Project Structure

```
Hospital-Management/
│
├── backend/
│   ├── index.js
│   ├── package.json
│   └── node_modules/
│
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── Hospital-Management-API.postman_collection.json
├── Hospital-Management.postman_environment.json
└── README.md
```

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/Hospital-Management.git
```

Move into the project directory

```bash
cd Hospital-Management
```

---

## 2. Install Backend Dependencies

```bash
cd backend
npm install
```

---

## 3. Install Frontend Dependencies

```bash
cd ../frontend
npm install
```

---

# 🗄 MongoDB Atlas Configuration

Open

```
backend/index.js
```

Replace

```javascript
const MONGODB_URI = "*";
```

with your MongoDB Atlas connection string.

Example:

```javascript
const MONGODB_URI =
"mongodb+srv://username:password@cluster.mongodb.net/hospitalDB";
```

---

# ▶️ Running the Application

## Start Backend

```bash
cd backend
node index.js
```

or

```bash
npm start
```

Backend runs at

```
http://localhost:5000
```

---

## Start Frontend

Open another terminal

```bash
cd frontend
npm run dev
```

Frontend runs at

```
http://localhost:5173
```

---

# 📡 REST API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/patients` | Get all patients |
| GET | `/patients/:id` | Get patient by ID |
| POST | `/patients` | Admit a patient |
| PUT | `/patients/:id` | Update patient details |
| DELETE | `/patients/:id` | Discharge patient |

---

# 📝 Sample Patient JSON

```json
{
  "name": "Ramesh Kumar",
  "age": 45,
  "gender": "Male",
  "disease": "Diabetes",
  "doctorAssigned": "Dr. Sharma",
  "roomNumber": "A-203"
}
```

---

# 🧪 API Testing

The repository includes:

- `Hospital-Management-API.postman_collection.json`
- `Hospital-Management.postman_environment.json`

### Import into Postman

1. Open Postman.
2. Click **Import**.
3. Import both JSON files.
4. Select the **Hospital Management - Local** environment.
5. Run the requests.

---

# 📸 Application Workflow

1. Enter patient details.
2. Click **Admit Patient**.
3. Patient is stored in MongoDB Atlas.
4. View patient list.
5. Search patients.
6. Edit patient information.
7. Delete (Discharge) patient.

---

# 📦 Dependencies

### Backend

```json
express
mongoose
cors
```

### Frontend

```json
react
vite
```

---

# Future Enhancements

- User authentication
- JWT authorization
- Doctor management
- Appointment scheduling
- Billing system
- Patient history
- Dashboard
