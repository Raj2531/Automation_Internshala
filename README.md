# 🤖 Internshala Automation

Ever had to fill out the same profile details and application questions again and again while applying for internships?

That was the idea behind this project.

I built this browser automation tool during a hackathon to automate some of the repetitive steps involved in managing an Internshala profile and applying for internships. The project uses **Node.js + Puppeteer** to control the browser and interact with Internshala.

## 💡 What does it do?

The automation handles a workflow starting from logging into Internshala and moving through different parts of the profile and application process.

It can:

* 🔐 Log into an Internshala account
* 🎓 Add/update educational details
* 📚 Add training information
* 🔗 Add portfolio/work sample links
* 🔎 Navigate through internship listings
* 📄 Open internship details
* ✍️ Fill application questions automatically
* 🚀 Submit internship applications

The profile information and application responses are kept separately in `data.js`, making it easier to customize the automation without changing the main logic.

## 🛠️ Tech Stack

* **JavaScript**
* **Node.js**
* **Puppeteer**
* **npm**

## ⚙️ How it works

```text
🚀 Start
   ↓
Launch Chromium
   ↓
🔐 Login to Internshala
   ↓
🎓 Update Education
   ↓
📚 Add Training
   ↓
🔗 Add Work Sample
   ↓
🔎 Browse Internships
   ↓
📄 Open Internship
   ↓
✍️ Fill Application
   ↓
🚀 Submit
```

Puppeteer handles the browser interactions while the information used during the workflow is maintained separately in `data.js`.

## 📁 Project Structure

```text
Automation_Internshala/
│
├── .gitignore
├── data.js
├── package.json
├── package-lock.json
├── script.js
└── README.md
```

### Important Files

**`script.js`** — Main Puppeteer automation logic.

**`data.js`** — Profile information and application responses.

**`package.json`** — Project configuration and dependencies.

**`.gitignore`** — Keeps sensitive and unnecessary local files out of Git.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Raj2531/Automation_Internshala.git
cd Automation_Internshala
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure your credentials

Use environment variables for your Internshala login credentials.

Create a local `.env` file:

```env
INTERNSHALA_ID=your_email
INTERNSHALA_PASSWORD=your_password
```

⚠️ Never commit your `.env` file or actual login credentials to GitHub.

### 4. Customize your data

Update `data.js` with the profile information and application responses you want the automation to use.

### 5. Run the project

```bash
node script.js
```

or:

```bash
npm start
```

Puppeteer will launch the browser and begin executing the automation workflow.

## 🧠 What I Learned

This project was a great introduction to browser automation and made me think about how repetitive tasks can be broken down into smaller, programmable steps.

While building it, I worked with:

* Browser automation using Puppeteer
* DOM selectors
* Form automation
* Asynchronous JavaScript
* Page navigation and dynamic elements
* Handling multi-step workflows
* Separating application logic from user data
* Managing sensitive credentials using environment variables

One of my biggest takeaways was that automation doesn't always have to be complicated. A workflow made up of many small repetitive actions can often be turned into a simple, reusable program.

## 🔮 Possible Improvements

* [ ] Add a proper UI instead of running everything from the terminal
* [ ] Add internship filtering based on user preferences
* [ ] Add better error handling and retry mechanisms
* [ ] Add application tracking
* [ ] Add detailed execution logs
* [ ] Generate application responses dynamically

## ⚠️ Disclaimer

This project was created for **learning and hackathon purposes**.

Websites can change their layouts, selectors, authentication systems, and workflows, which may require the automation to be updated.

Please use the project responsibly and in accordance with Internshala's applicable terms and policies.

---

Made with **JavaScript, Node.js, Puppeteer, and a lot of debugging. ☕💻**

