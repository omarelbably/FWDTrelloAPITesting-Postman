📬 FWDTrelloAPITesting-Postman

Welcome to FWDTrelloAPITesting-Postman — a complete API automation testing project for Trello, using Postman and Newman to validate the robustness and reliability of Trello’s RESTful APIs! 🚀🧪

    🎯 Ideal for both learners and professionals aiming to master API testing with Postman collections and automate them via CI/CD-ready scripts.

📚 About the Project

In today's agile world, API Testing is crucial to ensure seamless integration and performance across platforms.
This project showcases best practices for:

    🔗 Organizing scalable Postman collections

    🧪 Designing effective API test cases

    📊 Generating comprehensive reports

    ⚙️ Automating test execution with Newman (Postman CLI)

Test Focus Areas:

    🛠 Board Management (Create, Read, Update, Delete)

    🧹 List Management

    🗂 Card Operations

    🚫 Negative Testing (Authorization failures, Validation errors)

🛠️ Tech Stack

Technology	Purpose

Postman 🧡	API Collection and Testing

Newman 🛠️	Command-line Collection Runner

Node.js 📦	Runtime for Newman

Trello API 📬	Target API for Testing

JSON 📑	Data format for requests and responses

🚀 Getting Started

Follow these steps to quickly get the project running locally:
Prerequisites

    ✅ Node.js installed

    ✅ Postman installed

    ✅ Trello API Key & Token (Get them from your Trello API Keys page)

Setup Instructions

    Clone the Repository

git clone https://github.com/omarelbably/FWDTrelloAPITesting-Postman.git

    Navigate into the Project

cd FWDTrelloAPITesting-Postman

    Install Newman

npm install -g newman

    Set Your Environment

    Open Postman.

    Import the environment file provided (e.g., TrelloEnvironment.postman_environment.json).

    Update the environment variables:

        key — Your Trello API key

        token — Your Trello API token

    Import and Explore

    Import the collection file: TrelloAPITesting.postman_collection.json.

    Review and customize test cases if needed.

    Run the Collection Locally

newman run TrelloAPITesting.postman_collection.json -e TrelloEnvironment.postman_environment.json

✅ That's it — your API tests will now execute and results will be displayed on the terminal!

📂 Project Structure

FWDTrelloAPITesting-Postman/

├── TrelloAPITesting.postman_collection.json   # The Postman Collection

├── TrelloEnvironment.postman_environment.json # The Postman Environment

├── README.md                                  # Project Documentation

🔥 Project Highlights

✅ Organized requests grouped by functionality (Boards, Lists, Cards)

✅ Assertions on status codes, response times, and response body fields

✅ Environment-driven — easily switch between staging/production

✅ Supports Newman CLI Automation for CI/CD pipelines

✅ Clean, modular, and professional Postman structure

📡 Sample API Workflow

Action	Method	Endpoint

Create Board	POST	/1/boards/

Create List	POST	/1/lists/

Create Card	POST	/1/cards/

Update Card	PUT	/1/cards/{id}

Delete Board	DELETE	/1/boards/{id}

Each action is covered with validations to ensure both happy paths and edge cases are handled!

📊 Reports

Want prettier results? Use advanced reporting:

newman run TrelloAPITesting.postman_collection.json -e TrelloEnvironment.postman_environment.json -r cli,html

This will generate a beautiful HTML report 📄.
🧩 How to Contribute

We welcome community contributions! 💪

    Fork this repo 🍴

    Create your branch (git checkout -b feature/NewAwesomeTest)

    Commit your changes (git commit -m 'Add NewAwesomeTest')

    Push to the branch (git push origin feature/NewAwesomeTest)

    Open a Pull Request ✅

🎯 Roadmap

Build complete CRUD coverage for Trello

Setup Postman environment with dynamic variables

Integrate with Newman CLI

Automate execution via GitHub Actions/CI/CD pipelines 🚀

    Add detailed negative testing scenarios 🚫

📢 Contact

Omar Elbably
📧 Email: omaroelbably@gmail.com

🌐 GitHub: omarelbably

🌟 Show Your Support

If you find this project valuable, please ⭐ Star it — your support means everything! 🙏
Let's make API testing smarter, faster, and stronger together! 🚀✨

    Crafted with passion for APIs, testing, and automation excellence by Omar Elbably.

