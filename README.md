# Product Feedback App

## 👋 Welcome!

Imagine you are starting out as a freelance full-stack developer. You've just been hired by your first new client: a startup that is building a new product. The startup is generically named _My Company_. 

_My Company_ wants you to build a Product Feedback application, where customers can view and submit feedback about how their product could be improved. 

![image](https://github.com/user-attachments/assets/5fabe48e-fb2b-4337-94cc-515e64a0bf66)


## 🎯 Project Requirements

Users should be able to:

- View all product suggestions
- Submit a new product suggestions by filling out a form
- Receive form validations when trying to submit a new suggestion
- Filter suggestions by category
- When there are no suggestions for the currently selected filter, show the "There is no feedback" screen 
- View the optimal layout for the app depending on their device's screen size


## The Tech Stack

These are all the technologies you should use to build your full-stack application: 

| Component | Language | Framework | Deployment | Dev Tools |
|-----------|------------|----------------|------------|-------|
| Frontend  | HTML, CSS, JavaScript | React         | Netlify   |      |
| Server/API | Node.js     | Express       | Render    | Postman for API testing |
| Database  | PostgreSQL |               | Neon    |   |



## 🔗 Resources

- **Designs:** You will need to use this [Figma file](https://www.figma.com/design/ffyUs0kcwOG0gpe8N4BzYL/Product-Management-App?node-id=0-1&p=f&t=kSc9d10uZiSGCOFD-0) for the designs
- **Documentation Guides:** The teaching team at AnnieCannons has provided some [handy guides](https://docs.google.com/document/d/18jxCUA0bebCyYaIHy8aaKMgOQH4w5-b-iCGDWpV4K4M/edit?tab=t.0#heading=h.ykdbmvmlp0ag) to help you use Github and other coding tools



## 📝 Tips for building your project

1. **Pseudo-code before you write any code!** Look through the designs to plan out how you'll tackle the project. Write down your plan somewhere in this README or in your code. 
2. **Work on one feature at a time.** Finish one feature first before you move onto the next thing. Test as you go, routinely checking your site in the browser and making sure there are no errors before moving on. 
3. **Comment your code generously — Future You will thank you.** You’ll be building on top of this project over the next 3 months, so help yourself out by writing clear, helpful comments that explain what your code is doing. Trust us, it will save you time and confusion later.
4. **Clean up your code as you go**. Rename confusing variables, remove unused code, and organize your logic. Your code should read like a newspaper: clear, easy to follow, and understandable at a glance.


---

## 🚀 Roadmap: Step-by-step guide to building this project

---

### 🎯 Milestone: Create your database schema

1. Review the [Figma designs](https://www.figma.com/design/ffyUs0kcwOG0gpe8N4BzYL/Product-Management-App?node-id=0-1&p=f&t=kSc9d10uZiSGCOFD-0) and plan/pseudo-code what data you'll need to build this application 
2. [Fork this DB Fiddle](https://www.db-fiddle.com/f/mDJ76U1Xpi8ZR79RqDgYny/0)
3. Write PostgreSQL code to create your table(s)
4. Insert at least 3 rows of sample data into each table
5. Write the SQL queries for your API to:
     - Get all suggestions
     - Add a suggestion
6. Bookmark the link to your DB Fiddle so you can find it later.
7. Submit the link to your DB Fiddle on Canvas.
   
---

### 🎯 Milestone: Deploy the PostgreSQL database to Neon

1. Use Neon.tech to create a new Neon project called `suggestions`. Use this [Neon deployment guide](https://github.com/AnnieCannons/countries-api-project-may-2025/blob/main/version-4/deploy-database-to-neon.md) to help you. 
2. Set up your database on Neon (create your table(s) and insert rows of sample data)

---

### ⚙️ Fork & Clone the Github repo 
1. Fork this Github repo into your own account. Use this [fork and clone guide](https://docs.google.com/document/d/18jxCUA0bebCyYaIHy8aaKMgOQH4w5-b-iCGDWpV4K4M/edit?tab=t.55gk3qetux2a#heading=h.wbbot8ebr58a) to help you.
2. Clone your new Github repo into the `dev` folder on your local machine. 

---

### ⚙️ Set up your `server` folder in VS Code
1. In VS Code, open up your `product-feedback-app` project. You should see 3 folders and files already provided for you: 
     - `client` — holds your frontend React code
     - `server` — holds your backend server/API code
     - `README.md` — holds the project info & instructions
 
2. Open up the `server` folder. In that folder, you should see the following files already provided for you:

      - `package.json` — lists information about your project and its dependencies 
      - `.gitignore` — lists which files and folders that Git should ignore 
      - `src` folder — where all your custom code will live
      - `index.js` — where you will write your server/API code
      - `config.js` — contains your database's access credentials

3. In VS Code, open the terminal and `cd` into your `server` folder
4. In the `server` folder, run `npm install express` and `npm install pg`. 

     Once you do that, you should see `express` and `pg` listed as dependencies in your `package.json`. 

     You should also see your `node_modules` folder was generated. This folder contains all of the code from your project's dependencies. 

---

### ⚙️ Connect your Neon-hosted PostgreSQL database to your Express server
1. [Follow this guide to connect your Neon database to your Express server](https://github.com/AnnieCannons/countries-api-project-may-2025/blob/main/version-4/connect-neon-database-to-express-server.md).

---

### ⚙️ Set up your server's boilerplate code 
1. In your server's `index.js` file, set up your server using the same boilerplate code as the `06-recipe-API-server-SQL` project or your `version-4` of the Countries API project. 

---

### 🎯 Milestone: Build the server/API
1. `GET /get-all-suggestions`: Return all the suggestions data
2. `POST /add-one-suggestion`: Save submitted form data
3. Test your API endpoints in Postman to make sure they're working
4. Push your code to Github 

---

### 🎯 Milestone: Build the Frontend

1. Build the frontend in the `client` folder, according to the [Figma designs](https://www.figma.com/design/ffyUs0kcwOG0gpe8N4BzYL/Product-Management-App?node-id=0-1&p=f&t=kSc9d10uZiSGCOFD-0). Users should be able to:

   - View all product suggestions
   - Submit a new product suggestion by filling out a form
   - Receive form validations when trying to submit a new suggestion
   - Filter suggestions by category
   - When there are no suggestions for the currently selected filter, show the "There is no feedback" screen 
   - View the optimal layout for the app depending on their device's screen size
2. Push your code to Github

---

### 🎯 Milestone: Deploy the Frontend to Netlify and the Server/API to Render

1. Deploy your frontend code (in the `client` folder) to Netlify. Use this [Netlify deployment guide](https://docs.google.com/document/d/18jxCUA0bebCyYaIHy8aaKMgOQH4w5-b-iCGDWpV4K4M/edit?tab=t.jnwta4jrhylr#heading=h.scmsi7a6s9yz) to help you.
2. Deploy your server/API code (in the `server` folder) to Render. Use this [Render deployment guide](https://github.com/AnnieCannons/countries-api-project-may-2025/blob/main/version-5/README.md) to help you. 

---

### Test everything again... and again! 
1. Now that your database, API, and frontend are all deployed to the internet, you can test all user flows:
   - Viewing all suggestions
   - Filtering the suggestions
   - Adding a suggestion
3. Check your database to make sure the data is updating correctly

---

### Clean and Comment your code
1. Clean up your code to make it clean and modular
2. Remove unnecessary console.log() messages and unused blocks of commented-out code.
3. Comment complex logic to explain how it works

---

### 🎯 Milestone: Project Documentation 
1. In your project's README.md file, explain what your project is about, its tech stack, how to run it, etc. This is important if you intend to showcase this project on your resume or portfolio. Use this [README.md template](https://github.com/AnnieCannons/countries-api-project-may-2025/blob/main/version-5/writing-your-README.md) to help you write it! 

---

### Deploy & Submit
1. Push your code to Github
4. Submit to Canvas! You're done! 🎉

---

## 🌟 Stretch Goals (Optional)

Finished the main requirements? Here are some bonus challenges:

- 🏆 Upvote product suggestions
- 🏆 Sort suggestions by most/least upvotes and most/least comments
- 🏆 Edit an existing suggestion
- 🏆 Delete an existing suggestion
- 🏆 Add comments to an existing suggestion
