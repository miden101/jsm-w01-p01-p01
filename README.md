# 🎬 Cineplex

<p align="center">
  <img src="public/favicon.png" alt="Cineplex Logo" width="180" />
</p>

<p align="center">
  A movie discovery website built with React, Vite, JavaScript, TMDB, and Appwrite.
</p>

<p align="center">
  Discover popular movies, search for your favorites, and explore what's trending on Cineplex.
</p>

---

## ✨ Features

- **Popular Movies:** Browse the top 20 popular movies fetched from the TMDB API.
- **Movie Search:** Search for movies by title and discover relevant results.
- **Trending Movies:** Explore the top 5 trending movies based on search activity on Cineplex.
- **Search Analytics:** Track movie search counts using Appwrite.
- **Dynamic Trending Section:** Display movies according to their search frequency on the website.
- **Responsive Design:** Enjoy a movie-browsing experience across different screen sizes.
- **Loading & Error States:** Handle data loading and API errors to improve the user experience.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| React | Building the user interface |
| Vite | Development server and build tool |
| JavaScript | Application logic |
| CSS | Styling and responsive layouts |
| TMDB API | Fetching movie information and popular movies |
| Appwrite | Storing search statistics and retrieving trending data |
| Git & GitHub | Version control and source code hosting |
| Vercel | Deployment and hosting |

## 🎥 How It Works

### Popular Movies

Cineplex fetches popular movie data from the TMDB API and displays the top 20 results in the popular movies section.

### Search Movies

Users can search for movies by title. Cineplex fetches matching results from TMDB and displays them on the website.

### Trending Movies

The trending section highlights movies that visitors search for most frequently on Cineplex.

1. A user searches for a movie.
2. Cineplex records the search term and associated movie information in Appwrite.
3. Appwrite stores and maintains the search count.
4. Cineplex retrieves the five most frequently searched entries.
5. The trending section displays these entries to visitors.

Unlike the popular movies section, which uses TMDB's popularity data, the trending section reflects search activity on Cineplex.

## 🚀 Getting Started

### Prerequisites

Before running the project, ensure you have:

- [Node.js](https://nodejs.org/)
- npm
- A [TMDB account](https://www.themoviedb.org/) for API access
- An [Appwrite account](https://appwrite.io/) with a configured project and table

### Installation

**1. Clone the repository**

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

**2. Navigate to the project directory**

```bash
cd <YOUR_PROJECT_DIRECTORY>
```

**3. Install dependencies**

```bash
npm install
```

**4. Configure environment variables**

Create a `.env.local` file in the project root:

```env
VITE_TMDB_API_KEY=your_tmdb_api_key
VITE_APPWRITE_ENDPOINT=your_appwrite_endpoint
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_TABLE_ID=your_appwrite_table_id
```

Replace the placeholder values with your actual credentials and configuration. The variable names must match those referenced in your source code.

**5. Start the development server**

```bash
npm run dev
```

Open the local URL displayed in your terminal to start exploring Cineplex.

### Production Build

Create an optimized production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

## 🔐 Environment Variables & Security

- Keep `.env.local` private and excluded from version control.
- Never commit API keys or credentials to a public repository.
- Configure the required environment variables in your Vercel project settings.
- Review Appwrite table permissions before deploying publicly.
- Remember that Vite variables prefixed with `VITE_` are exposed to client-side code and must not contain private server secrets.

## 🌐 Live Demo

- **Live Website:** <YOUR_DEPLOYED_WEBSITE_URL>
- **GitHub Repository:** <YOUR_GITHUB_REPOSITORY_URL>

## 📚 What I Learned

Building Cineplex helped me gain practical experience with:

- Developing a React application using Vite.
- Fetching and displaying data from a third-party REST API.
- Managing application state and user input.
- Integrating Appwrite with a frontend application.
- Recording search activity and implementing a trending system.
- Managing environment variables.
- Using Git and GitHub for version control.
- Building and deploying a production-ready frontend application.

## 🙏 Acknowledgements

- [TMDB](https://www.themoviedb.org/) — Movie data and API.
- [Appwrite](https://appwrite.io/) — Backend services and data storage.
- [React](https://react.dev/) — UI library.
- [Vite](https://vite.dev/) — Development and build tooling.

This product uses the TMDB API but is not endorsed or certified by TMDB.

---

<p align="center">
  <strong>Cineplex</strong> — Discover your next favorite movie. 🍿
</p>
