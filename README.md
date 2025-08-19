# 7-Days-of-JS
contains theory, explanations, assignments and a single project improved daily

---
# 📝 General Prompt Template
## Prompt:
I want to work on [describe your goal or project clearly].
It should include the following features or requirements:
- [Feature 1]
- [Feature 2]
- [Feature 3]
  
👉 Please give me a structured and prioritized list of [topics/steps/tools/skills/resources] I need to learn or use to achieve this.

---
# How i used it for creating this course
## propmt:
- I want to build a Next.js final year project with the following features:
- Resume Builder
- AI-generated Cover Letter
- AI-powered Study Planner
- Job Market Analysis for Current Trends
- Mock MCQs for a Particular Domain (AI-generated)
- AI Interview with a Voice Agent
- Interview & Performance Analysis
- Before starting, I need to learn JavaScript (and related concepts) required for this project.
  
👉 Please give me a structured list of JavaScript and essential Next.js topics I should learn, focusing only on what will actually be used in this project. Do not include unnecessary or unrelated topics.


---
# Day 1 – JS Foundations (Resume Form Basics)
## 🎓 Theory

Variables & Data Types: let, const
👉 Industry Use: Storing API keys securely, tracking app state.
👉 Creative Use: A "mood tracker" app that stores today’s mood in a variable.

Conditionals & Loops: if, else, switch, for, while
👉 Industry Use: Validating forms (e.g., email format).
👉 Creative Use: A “study reminder” loop that checks the current time and alerts you.

## 📝 Assignments

Create a program that checks if a student passed based on marks (>= 40 = Pass).

Write a loop that prints the first 10 even numbers.

## 🏗️ Project Task

Create a basic resume form with fields: Name, Email, Skills.

Use conditionals to validate: email must include @, skills should not be empty.

---

# Day 2 – Functions & Arrays (Resume Skills Section)
## 🎓 Theory

Functions: Reusable blocks, arrow functions.
👉 Industry Use: Utility functions in React (e.g., format dates).
👉 Creative Use: A random “study break suggestion” generator.

Arrays & Methods (map, filter, reduce)
👉 Industry Use: Filtering job listings by domain.
👉 Creative Use: Aggregating study hours for a week.

# 📝 Assignments

Write a function that calculates the average of an array of numbers.

Given an array of job roles, filter only those containing "Engineer".

# 🏗️ Project Task

Add a Skills Section to your resume builder:

Enter multiple skills (store in an array).

Display them using map().


---

# Day 3 – Objects & Destructuring (Job Data Handling)
## 🎓 Theory

Objects: Key-value pairs to store structured data.
👉 Industry Use: User profiles ({name, email, skills}).
👉 Creative Use: AI “study persona” with {focusLevel, preferredTime, strengths}.

Destructuring & Spread
👉 Industry Use: Extract API response data.
👉 Creative Use: Merge two resumes into one mega-resume with spread operator.

# 📝 Assignments

Create an object for a student with name, age, and grades. Access the properties with destructuring.

Merge two objects: {a:1, b:2} and {c:3} → {a:1, b:2, c:3}.

# 🏗️ Project Task

Store all resume data (name, email, skills) inside an object.

Use destructuring to display it neatly on the page.

---


# Day 4 – Async JS (AI Cover Letter & Job Trends)
# 🎓 Theory

Promises, async/await, fetch API
👉 Industry Use: Fetching job data from LinkedIn/Indeed API.
👉 Creative Use: Fetching a motivational quote before every study session.

# 📝 Assignments

Fetch a random joke from https://official-joke-api.appspot.com/random_joke. Display setup and punchline.

Write an async function that waits 2 seconds, then logs “Study Time!”.

# 🏗️ Project Task

Add a Cover Letter Generator section:

Use fetch() to call a dummy AI API (mock it with JSONPlaceholder or hardcoded text).

Display generated cover letter below resume.

Add Job Trends Section that fetches and displays trending job titles.

---

# Day 5 – Storage & Error Handling (Save Resume Drafts)
## 🎓 Theory

localStorage: Save and load data.
👉 Industry Use: Saving user login state.
👉 Creative Use: Save today’s study plan automatically.

try/catch: Handle failed API calls.
👉 Industry Use: Handle failed payment gateway request.
👉 Creative Use: “Fallback study task” if AI planner API fails.

# 📝 Assignments

Store a user’s name in localStorage and retrieve it on page reload.

Write a fetch function with try/catch to handle API errors gracefully.

#🏗️ Project Task

Add Save Draft feature for resume builder using localStorage.

If API fails (job trends or cover letter), show a custom error message.


---
# Day 6 – Voice & MCQs (AI Interview Prep)
## 🎓 Theory

Web Speech API: Speech recognition, text-to-speech.
👉 Industry Use: Voice chatbots (like Alexa, Google Assistant).
👉 Creative Use: A “study narrator” that reads your notes aloud.

Timers (setTimeout, setInterval)
👉 Industry Use: Quiz countdown timer.
👉 Creative Use: Pomodoro study timer.

# 📝 Assignments

Build a timer that counts down from 10 and prints “Time’s up!”.

Use the Speech Synthesis API to make your browser say: “Welcome to AI Interview”.

# 🏗️ Project Task

Add Mock MCQ Quiz:

Show 5 MCQs with options.

Add a timer for the quiz.

Add AI Interview Section:

Use Speech API to ask a question.

Capture student’s voice as an answer.

---

# Day 7 – Integration & Analysis Dashboard
## 🎓 Theory

Modules & Clean Code
👉 Industry Use: Splitting features into separate files in Next.js apps.
👉 Creative Use: A “plugin system” for study tools.

## 📝 Assignments

Export a function from one file and import it in another.

Organize resume, MCQ, and job-trend logic into separate files.

## 🏗️ Final Project Task

Integrate everything into one Next.js app:

Resume Builder (+ Save Draft)

AI Cover Letter Generator

AI Study Planner (dummy data or API)

Job Trends Analysis (fetch job data)

MCQ Mock Test with timer

AI Voice Interview (ask & record answers)

Analysis Dashboard → show:

Resume completeness %

Quiz score

Interview transcript
