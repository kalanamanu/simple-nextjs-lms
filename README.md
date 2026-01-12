# Learning Management System (LMS)

## 📌 Project Overview

This project is a **full-stack Learning Management System (LMS)** built to strengthen and refresh core software engineering fundamentals, including **Next.js, Node.js, MongoDB, JWT authentication**, and frontend development using **TypeScript and Tailwind CSS**.

The system supports **role-based access control** and simulates a real-world LMS workflow involving **Admins, Instructors, and Students**.

---

## 🎯 Project Goals

- Practice full-stack development with a clear separation of frontend and backend
- Implement JWT-based authentication and role-based authorization
- Design and implement MongoDB data models
- Build real-world CRUD operations
- Strengthen understanding of request–response flow and data relationships

---

## 🧑‍💼 User Roles

- **Admin**
- **Instructor**
- **Student**

---

## 🔑 Core Features (v1)

### Authentication & Authorization

- User registration and login
- JWT-based authentication
- Role-based access control

### Course Management

- Admin creates courses
- Admin assigns instructors to courses
- Admin sets maximum student capacity for courses
- Instructor adds lessons to assigned courses

### Enrollment Management

- Instructor manually enrolls students into courses
- Enrollment capacity is enforced based on course limits

### Learning Progress

- Students can manually mark lessons as completed
- Lesson completion is tracked per student

### Dashboards

- Role-based dashboards for Admin, Instructor, and Student

---

## 🛠 Tech Stack

### Frontend

- Next.js (App Router)
- TypeScript
- Tailwind CSS

### Backend

- Node.js
- Express.js

### Database

- MongoDB
- Mongoose ODM

### Authentication

- JSON Web Tokens (JWT)
- bcrypt

---

## 🗂 Project Structure

### Backend

lms-backend/
├── src/
│ ├── models/
│ ├── controllers/
│ ├── routes/
│ ├── middleware/
│ ├── config/
│ └── server.js


### Frontend

lms-frontend/
├── app/
│ ├── login/
│ ├── register/
│ ├── dashboard/
│ ├── courses/
│ └── layout.tsx


---

## 🧱 Database Design

### User

\_id

name

email

password

role (admin | instructor | student)


### Course

\_id

title

description

instructorId (User)

maxStudents

createdBy (Admin)

shell
Copy code

### Lesson

\_id

title

content

courseId (Course)

shell
Copy code

### Enrollment

\_id

userId (Student)

courseId (Course)

enrolledAt


### LessonProgress

\_id

userId (Student)

lessonId (Lesson)

completed

completedAt


---

## 🔄 System Workflow

1. Admin creates a course and assigns an instructor
2. Instructor adds lessons and enrolls students
3. Students view lessons and mark them as completed
4. Lesson progress is stored per student

---

## 🤖 AI Usage Policy

AI tools are used **only for explanation, debugging, and concept clarification**.  
All implemented code is reviewed and understood before being committed.

---

## 🚀 Future Enhancements (v2)

- Course completion tracking
- Certificates
- Quizzes and assessments
- Payment integration
- Notifications

---

## 📚 Learning Focus

This project focuses on:

- Backend-first development
- Clear data modeling
- Authentication and authorization
- Understanding full request flow
- Writing maintainable and explainable code

---

## 📌 Status

**In Progress** — actively developed while applying for junior/graduate software engineering roles.
