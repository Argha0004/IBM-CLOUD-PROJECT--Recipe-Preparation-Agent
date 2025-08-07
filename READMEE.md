Check In Windows Command Prompt

# 🍳 Recipe Preparation Agent

A modern, AI-driven web application developed with **Node.js** and powered by **IBM Granite LLM** to help you transform your pantry ingredients into delicious, complete recipes.

---

## 🚀 Features

- **AI-Generated Recipes**: Just type in what you have — get instant, complete dishes  
- **Guided Cooking**: Clear, step-by-step instructions for every recipe  
- **Ingredient Alternatives**: Offers smart replacements for missing ingredients  
- **Expert Tips**: Pro insights to level up your cooking  
- **Nutritional Insights**: Basic nutritional breakdown included  
- **Modern Aesthetic**: Sleek, responsive design with Tailwind CSS  
- **Quick Copy**: One-click button to copy and share the recipe easily  

---

## 🛠️ Tech Stack

- **Backend Framework**: Node.js with Express  
- **LLM Support**: IBM Granite LLM via Watson Machine Learning APIs  
- **Frontend Tools**: HTML, Tailwind CSS, JavaScript  
- **Styling Method**: Tailwind CSS with custom enhancements  

---

## 📦 Getting Started

### Requirements

- Install Node.js (v16 or above)  
- Create an IBM Cloud account with Watson Machine Learning service  
- Obtain IBM Watson ML credentials

### Setup Instructions

1. **Clone This Project**
   ```bash
   git clone <repository-url>
   cd recipe-preparation-agent
   ```

2. **Install Required Packages**
   ```bash
   npm install
   ```

3. **Environment Setup**
   - Duplicate `.env.example` as `.env`
   - Provide the necessary IBM credentials:
     ```
     IBM_WATSON_ML_API_KEY=your_api_key
     IBM_WATSON_ML_URL=https://us-south.ml.cloud.ibm.com
     IBM_WATSON_ML_PROJECT_ID=your_project_id
     ```

4. **Run the Application**
   ```bash
   npm start
   ```

5. **Open in Browser**
   - Go to `http://localhost:5000`

---

## 🔐 How to Obtain IBM Watson ML Credentials

1. **Register on IBM Cloud**
   - Visit [IBM Cloud](https://cloud.ibm.com/) to sign up

2. **Provision a Watson Machine Learning Service**
   - From the dashboard:  
     - Click **Create Resource**, search for *Watson Machine Learning*  
     - Choose the **Lite** (free) plan and create the instance

3. **Generate Your API Key**
   - Go to your ML instance → **Service Credentials**  
   - Create new credentials → Copy the `apikey`

4. **Locate Your Project ID**
   - Go to [Watson Studio](https://dataplatform.cloud.ibm.com/)  
   - Create a new project, then check its **Settings** for the **Project ID**

---

## ⚙️ Using the App

1. Input your available ingredients (like `tomato, garlic, onion`)  
2. Click the **Generate Recipe** button  
3. Receive:
   - A full recipe with quantities  
   - Cooking instructions  
   - Ingredient substitutes  
   - Helpful tips and nutrition information  
4. Use **Copy** to save or share with ease

---

## ✨ Sample Inputs

| Your Ingredients                   | Recipe Output                 |
|-----------------------------------|-------------------------------|
| `tomato, onion, rice`             | Tomato Rice Pilaf             |
| `chicken, garlic, lemon, herbs`   | Herb-Crusted Lemon Chicken    |
| `pasta, mushrooms, cream`         | Creamy Mushroom Pasta         |
| `eggs, spinach, cheese`           | Spinach & Cheese Omelet       |

---

## 📡 API Overview

- `GET /` → Loads the main interface  
- `POST /generate-recipe` → Triggers AI recipe generation  
- `GET /health` → Simple health check endpoint

---

## 📁 Folder Structure

```
recipe-preparation-agent/
├── server.js              # Main Express server file
├── package.json           # Project dependencies
├── .env.example           # Example environment config
└── public/
    ├── index.html         # Frontend structure
    ├── js/
    │   └── app.js         # Core frontend logic
    └── css/
        └── style.css      # Tailwind and custom styles
```

---

## 🧠 In-Depth AI Functionality

### Intelligent Recipe Crafting
- IBM Granite LLM crafts realistic and creative recipes  
- Combines user inputs with culinary logic and common pairings

### Clean and Clear Output
- Recipes are well-structured and easy to follow  
- Highlights essential parts for user clarity

### Optimized for Mobile
- Fully responsive layout for phones, tablets, and desktops  
- UI scales seamlessly across screen sizes

---

## 🧩 Common Issues & Fixes

### Facing API Credential Errors?
- Recheck your `.env` file for typos  
- Ensure your IBM Watson ML instance is live  
- Confirm your Project ID is correctly entered

### Recipe Not Appearing?
- Test your internet connectivity  
- Try entering basic ingredients  
- Check IBM Cloud status in case of service interruptions

### UI or Style Not Loading?
- Ensure Tailwind CSS is properly linked  
- Use browser dev tools to inspect for console errors  
- Clear cache or reload the app

---

## 🤝 Contribution Guide

1. Fork the repository  
2. Create a feature-specific branch  
3. Test and commit your changes  
4. Submit a Pull Request (PR) with details

---

## 📄 License

This project is open-source and licensed under the MIT License.  
See the `LICENSE` file for full terms.

---

## 📬 Need Help?

For support:  
- See the [Troubleshooting](#-common-issues--fixes) section  
- Explore [IBM Watson ML Docs](https://cloud.ibm.com/docs/watson-machine-learning)  
- Or raise an issue on the GitHub repo

---

**Created with ❤️ using Node.js, Tailwind CSS, and IBM Granite LLM**  
Part of IBM-CLOUD-EDUNET
