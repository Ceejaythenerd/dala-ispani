Dala Ispani - Sketch Your Future ✍️

Dala Ispani (South African slang for "Make the job work" or "Make the hustle happen") is a vibrant, youth-focused employment platform designed with a unique "Sketchbook" aesthetic. It connects young people in Mzansi to Learnerships, Internships, and Vacancies.

🎨 Design Philosophy

The site moves away from sterile corporate designs, utilizing a hand-drawn, notebook style. It features:

Lined paper backgrounds and sticky notes.

Handwritten typography (Amatic SC & Patrick Hand).

Doodle SVG icons (Stickmen, arrows, and food).

Interactive elements like scribbled buttons and highlighter effects.

✨ Key Features

Dynamic Job Board:

Jobs are rendered via JavaScript from a central data object (db).

Supports three distinct categories: Learnerships, Internships, and Vacancies.

Smart Filtering:

Search Bar: Real-time text filtering by job title or company.

Category Pills: Filter by sector (Retail, Tech, Admin, Logistics, etc.).

Saved Jobs (Local Storage):

Users can "Heart" ❤️ a job to save it.

Saved status persists even if the browser is refreshed.

Dedicated filter to view only saved jobs.

Social Sharing:

Integrated WhatsApp Share button in job details to easily share opportunities with friends.

CV Cheat Sheet:

A built-in modal providing quick, actionable tips for improving CVs.

"Buy Me a Kota" Support:

A fun, localized call-to-action on the desktop sidebar to support the site creators.

🚀 Getting Started

Prerequisites

You do not need to install Node.js or any backend servers. This is a static web application.

Installation

Download the project files.

Ensure you have an internet connection (required to load Tailwind CSS and Google Fonts).

Open index.html in any modern web browser (Chrome, Edge, Firefox, Safari).

⚙️ Configuration & Updates

Updating Job Data

The job listings are stored in a JavaScript constant named db located at the bottom of index.html.

To add a new job:

Open index.html in a text editor (VS Code, Notepad++, etc.).

Scroll down to the <script> tag.

Add a new object to the relevant array (learnerships, internships, or vacancies).

Example Data Structure:

{
    id: 10, // Must be unique
    title: "New Job Title",
    category: "Tech", // For filtering
    company: "Company Name",
    location: "JHB",
    salary: "R10,000",
    type: "Full Time", // or Contract/Part-time
    description: "Job description goes here...",
    requirements: ["Req 1", "Req 2"],
    applyLink: "[https://external-application-link.com](https://external-application-link.com)",
    icon: "fa-laptop", // FontAwesome icon class
    color: "blue-100" // Optional: 'blue-100' or 'pink-100' for sticky note color
}


Automation (Advanced)

To automate updates:

Move the db variable content to a separate file (e.g., data.json).

Update the JavaScript to fetch('data.json') on load.

Write a scraper (Python/Node.js) that runs daily, scrapes job portals, and updates data.json.

Customizing Links

Buy Me a Kota: Search for <!-- Update href below... --> in the HTML and replace # with your actual profile link.

🛠️ Built With

HTML5: Semantic structure.

Tailwind CSS (CDN): Rapid styling and responsive design.

Vanilla JavaScript: Data rendering, modal logic, and local storage management.

FontAwesome: Icons.

Google Fonts: Custom typography.

📄 License

This project is open-source. Feel free to modify and distribute.

Made with ❤️ in Mzansi.
