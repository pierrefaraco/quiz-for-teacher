# Quiz For Teacher

This is an old Java project I built for the **GLG204** module at **CNAM** (Conservatoire National des Arts et Métiers).

## Principle

The app lets a teacher (the "professor") create courses and quizzes, and lets students (the "auditors") join and answer them live, similar to Kahoot:

- A professor creates a **course**, organizes it into **topics/sequences**, and writes multiple-choice **questions** for each one.
- Students **subscribe** to a course.
- The professor starts a **quiz session** for the course; subscribed students join that session and answer the questions in real time over **WebSocket**.
- Answers are collected and scored, and the professor can consult **statistics** (per-student and per-question results) once the session ends.

## Tech stack

- **Backend**: Java, Spring MVC, Spring Security, Hibernate/JPA, MySQL, exposed as a REST API + WebSocket endpoint.
- **Frontend**: AngularJS single-page app (separate views/routes for the professor and the auditor).
- Built with Maven, packaged as a WAR for deployment on a servlet container (e.g. Tomcat).    
test
