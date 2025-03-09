# AI-Powered Job Portal

## Overview
The **AI-Powered Job Portal** is a full-stack web application built using the **MERN (MongoDB, Express.js, React.js, Node.js) stack**. It leverages **Artificial Intelligence (AI) and Natural Language Processing (NLP)** to extract key skills and experience from user-uploaded resumes and provide AI-driven job recommendations.

## Features
- **User Authentication:** Secure login and registration using JWT.
- **Resume Parsing:** Extracts skills and experience from uploaded resumes using NLP.
- **AI-Driven Job Recommendations:** Matches job seekers with relevant jobs based on extracted data.
- **Job Search & Applications:** Users can search for jobs, apply, and track applications.
- **Recruiter Dashboard:** Employers can post jobs, manage listings, and view ranked candidates.
- **Role-Based Access Control:** Separate dashboards for job seekers and recruiters.
- **Real-Time Notifications:** Get notified about job updates and application status.
- **Advanced Search & Filters:** AI-powered filtering to match job preferences.

## Tech Stack
### Frontend
- React.js (UI Framework)
- Redux (State Management)
- Bootstrap / Tailwind CSS (Styling)

### Backend
- Node.js (Runtime Environment)
- Express.js (Web Framework)
- MongoDB (Database)
- Mongoose (ORM)
- JWT (Authentication)

### AI/ML Technologies
- NLP (Natural Language Processing) for resume parsing
- TF-IDF & Cosine Similarity for job recommendations
- Pretrained AI models for skill extraction

## Installation & Setup
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
2. **Install Dependencies**
   ```sh
   npm install
   cd client && npm install
   ```
3. **Set Up Environment Variables**  
   Create a `.env` file in the root directory and add the following:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   PORT=5000
   ```
4. **Run the Server**
   ```sh
   npm run dev
   ```
5. **Run the Frontend**
   ```sh
   cd client
   npm start
   ```

## API Endpoints
### User Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login with email & password

### Job Management
- `POST /api/jobs/create` - Recruiters can post a new job
- `GET /api/jobs/` - Retrieve job listings
- `GET /api/jobs/recommend` - Get AI-powered job recommendations

### Resume Processing
- `POST /api/resume/upload` - Upload and parse a resume
- `GET /api/resume/data` - Get extracted skills & experience

## Contribution
Feel free to contribute to the project by creating a fork and submitting a pull request.

## License
This project is licensed under the MIT License.

