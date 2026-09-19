# NEXORA - Node.js Express EJS Landing Page

A modern, responsive landing page built with **Node.js, Express.js and EJS**.  
The project uses EJS for rendering the webpage and a separate CSS file for the black-and-white responsive design.

## 🚀 Project Overview

**NEXORA** is a modern digital workspace landing page. It includes:

- Responsive navigation bar
- Hero section
- Dashboard preview
- Trust/brand section
- Features section
- How It Works section
- Statistics section
- Customer reviews
- FAQ section
- Final call-to-action section
- Footer
- Responsive design for desktop, tablet and mobile

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Node.js | JavaScript runtime |
| Express.js | Web server and routing |
| EJS | Server-side HTML templating |
| HTML5 | Page structure |
| CSS3 | Styling and responsive design |
| Nodemon | Automatically restarts the server during development |

## 📁 Folder Structure

```text
node_pr-3-con_html/
│
├── Controllers/
│   └── HomeController.js
│
├── public/
│   └── css/
│       └── style.css
│
├── View/
│   └── home.ejs
│
├── index.js
├── package.json
├── package-lock.json
└── README.md
```

### Folder and File Explanation

#### `Controllers/`

Contains the controller logic for handling application requests.

```text
Controllers/
└── HomeController.js
```

`HomeController.js` handles the `/home` route and renders the `home.ejs` page.

#### `public/`

Contains static files that can be directly served to the browser.

```text
public/
└── css/
    └── style.css
```

`style.css` contains the complete styling, layout, colors, animations, cards and responsive media queries.

#### `View/`

Contains EJS templates.

```text
View/
└── home.ejs
```

`home.ejs` contains the complete HTML structure of the NEXORA landing page.

#### `index.js`

This is the main server file.

It:

- Imports Express
- Imports the Home controller
- Sets EJS as the view engine
- Sets the `View` folder as the views directory
- Serves files from the `public` folder
- Creates the `/home` route
- Starts the server on port `3000`

#### `package.json`

Contains project information, dependencies and npm scripts.

Main dependencies:

- `express`
- `ejs`
- `nodemon`

#### `package-lock.json`

Stores the exact dependency versions installed for the project.

## 🔄 Application Flow

The request flow of this project is:

```text
Browser
   │
   │  GET /home
   ▼
index.js
   │
   ▼
app.get('/home', home)
   │
   ▼
HomeController.js
   │
   ▼
res.render('home')
   │
   ▼
View/home.ejs
   │
   ▼
HTML + CSS
   │
   ▼
Browser Output
```

## 📱 Responsive Design

The CSS includes media queries for smaller screens.

The page adapts to:

- Desktop
- Laptop
- Tablet
- Mobile

The navigation, feature cards, statistics, testimonials, FAQ and footer adjust automatically based on screen size.

## 🖥️ Main Page Sections

### 1. Navbar

Contains:

- NEXORA logo
- Home
- Features
- How It Works
- Reviews
- Contact
- Get Started button

### 2. Hero

Main slogan:

> Work smarter. Move faster.

Includes a call-to-action and dashboard preview.

### 3. Features

Four main features:

- Smart Organization
- Real-Time Collaboration
- Powerful Insights
- Faster Workflow

```

## 👨‍💻 Author

**Yash**

## 📄 License

This project currently uses the **ISC** license as specified in `package.json`.

