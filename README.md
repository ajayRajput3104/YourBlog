# 📝 React Blog App

A full-featured blog application .This project demonstrates how to build a modern blog platform using React with real-time backend services powered by Appwrite.💙

## 🚀 Features

- 🔐 **Authentication** – Sign up, login, logout using Appwrite
- ✍️ **Create Posts** – Add blog posts with rich-text editing using TinyMCE
- 📃 **Read Posts** – View:
  - Your own posts (active & inactive)
  - All users’ public (active) posts
- 🔄 **Update Posts** – Edit your own blog content
- ❌ **Delete Posts** – Delete your posts with ease
- 📄 **Post Status Management** – Toggle between Active/Inactive visibility

## 🛠️ Tech Stack

| Frontend               | Backend / Services               |
|------------------------|----------------------------------|
| React                  | Appwrite (Auth, Database, Storage) |
| Redux Toolkit          |                                  |
| React Router DOM       |                                  |
| React Hook Form        |                                  |
| TinyMCE Rich Text Editor |                                |
| Tailwind CSS           |                                  |

## 📁 Folder Structure (Simplified)
```
src/
│
├── AppWrite/             # Appwrite API integration and services(Authorisation and storage)
├── Components/           # Reusable UI components (Header,Footer,AuthLayout, Input, Button, etc.)
├── conf/                 # `conf.js` – Centralized configuration file for environment variables used throughout the app (Appwrite project, database, bucket, TinyMCE API, etc.).
├── store/                # Redux slices and state logic
├── pages/                # Route-based pages (Home, Login, Signup, AllPosts, AddPost, EditPost)
├── App.jsx               # Main layout component; manages user auth on load, shows header/footer, and routes content with <Outlet />
└── main.jsx              # Entry point of the app that sets up routing, Redux store, and renders the root component.
```

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/react-blog-app.git
cd react-blog-app
```
### 2. Install dependencies
```bash
npm install
```
### 3. Configure Appwrite
Create a project on Appwrite Cloud

Enable Authentication, Database, and Storage

Set up the following environment values in .env file:
```js
export const conf = {
  appwriteUrl: "https://cloud.appwrite.io/v1",
  appwriteProjectId: "your_project_id",
  appwriteDatabaseId: "your_database_id",
  appwriteCollectionId: "your_collection_id",
  appwriteBucketId: "your_bucket_id",
};
```
### 4. Run the App
```bash
npm run dev
```
The application should now be running on http://localhost:5173.
### 🌱 Learning Outcomes
-Built a complete blog platform using React from scratch

-Understood how to use Redux Toolkit for efficient state management

-Learned routing and protected routes using React Router

-Integrated Appwrite as a BaaS (Backend as a Service)

-Used TinyMCE to enable rich-text editing

-Practiced modular and scalable project structuring

### 🛸 Deployment
You can deploy this app easily on platforms like Vercel or Netlify.

## 🔒 Authentication & Authorization
-All posts are private by default (Inactive)

-Only logged-in users can create, edit, or delete their own posts

-Only active posts are visible to the public

-Edit and Delete buttons appear only for the post author

### 🤝 Acknowledgements
This project was built as part of the [Chai aur Code](https://www.youtube.com/@chaiourcode) React series by [@hiteshdotcom](https://twitter.com/hiteshdotcom).
Special thanks to Hitesh Choudhary for the wonderful Chai aur Code series that inspired this project.

### 💬 Feedback or Suggestions?
This is a learning project and I’m open to all feedback! Feel free to fork, open issues, or submit pull requests.

📜 License
This project is open-sourced under the MIT License.
```vbnet

Let me know if you want to add:
- A live demo link
- Screenshots or GIFs of the app in action
- API schema or database structure overview  
I'll help plug them in cleanly.
```
