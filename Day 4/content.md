# 📅 Day 4: Async JS (AI Cover Letter & Job Trends)
## 🎓 Theory
1. Promises

A Promise is an object representing the eventual completion (or failure) of an async task.

States: pending → fulfilled → rejected.

const jobPromise = new Promise((resolve, reject) => {
  let dataFetched = true;
  if (dataFetched) {
    resolve("Jobs fetched successfully!");
  } else {
    reject("Error fetching jobs");
  }
});

jobPromise.then(msg => console.log(msg)).catch(err => console.error(err));

2. async/await

Cleaner syntax for handling promises.

await pauses execution until the Promise resolves.

async function fetchJob() {
  try {
    let response = await fetch("https://jsonplaceholder.typicode.com/posts/1");
    let data = await response.json();
    console.log("Job Data:", data);
  } catch (error) {
    console.error("Error:", error);
  }
}
fetchJob();

3. Fetch API

Used to make network requests (like APIs).

Returns a Promise.

fetch("https://jsonplaceholder.typicode.com/posts")
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(err => console.error("Error:", err));

#c🌍 Industry Use

Job Portals (LinkedIn, Indeed) → Use async fetch to pull job listings.

AI Recruiting Tools → Generate cover letters on demand with APIs.

#💡 Creative Use

Show a motivational quote or meme every time you open your study dashboard.
(Like “Keep going, future SDE at Amazon!” 😄)

# 📝 Assignments

Fetch Joke API

Fetch a random joke and display setup and punchline.

async function getJoke() {
  let res = await fetch("https://official-joke-api.appspot.com/random_joke");
  let data = await res.json();
  console.log(`${data.setup} - ${data.punchline}`);
}
getJoke();


Async Timer

async function studyReminder() {
  await new Promise(resolve => setTimeout(resolve, 2000));
  console.log("📚 Study Time!");
}
studyReminder();

# 🏗️ Project Task
## 1. Cover Letter Generator Section

Mock AI API using JSONPlaceholder.

Example: Fetch dummy text as a "cover letter".

async function generateCoverLetter() {
  let res = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  let data = await res.json();
  
  document.getElementById("cover-letter").innerText =
    `Dear Recruiter,\n\n${data.body}\n\nRegards,\n[Your Name]`;
}


HTML:

<button onclick="generateCoverLetter()">Generate Cover Letter</button>
<pre id="cover-letter"></pre>

## 2. Job Trends Section

Simulate fetching trending job titles.

async function fetchJobTrends() {
  let res = await fetch("https://jsonplaceholder.typicode.com/posts?_limit=5");
  let jobs = await res.json();
  
  let list = document.getElementById("job-trends");
  list.innerHTML = "";
  
  jobs.forEach(job => {
    let li = document.createElement("li");
    li.textContent = `🔥 Trending: ${job.title}`;
    list.appendChild(li);
  });
}


HTML:

<button onclick="fetchJobTrends()">Show Job Trends</button>
<ul id="job-trends"></ul>
