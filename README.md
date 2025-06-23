# 🎬 Movie Finder App

![React](https://img.shields.io/badge/Built%20With-React-blue.svg)
![API](https://img.shields.io/badge/API-TMDB-informational)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

A sleek and dynamic movie search application built with React that helps users discover trending and popular movies instantly using **The Movie Database (TMDb)** API.

> “Find movies you'll enjoy without the hassle.” — Your new favorite movie app.

---

## 📸 Demo

![Movie App Demo](https://your-demo-link-or-gif-here.gif)

> _Replace the above link with a demo video or GIF if available._

---

## ✨ Features

- 🔍 **Search any movie** with instant suggestions (debounced search)
- 🎞️ **Trending movies** section powered by TMDb API
- ⚡ **Fast and responsive** UI using functional components
- ⏳ **Loading spinner** for better user experience
- 📈 **Search analytics** integration with Appwrite (via `updateSearchCount`)
- 🧠 Smart API error handling and feedback

---

## 🛠️ Tech Stack

- **React.js**
- **TMDb API**
- **Appwrite (Backend for tracking search count)**
- **Custom Hooks (react-use's `useDebounce`)**
- **TailwindCSS / Custom CSS (assumed for styling)**

---

## 🧩 Project Structure

```
src/
├── components/
│   ├── MovieCard.jsx          # Renders each movie card
│   ├── Search.jsx             # Search input component
│   └── Spinner.jsx            # Loader while data is being fetched
├── App.jsx                    # Main app logic and UI rendering
├── appwrite.js                # Functions to fetch trending movies and update search counts
└── main.jsx                   # React DOM entry point
```

---

## 🔧 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-finder-app.git
cd movie-finder-app
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env` file in the root directory:

```
VITE_TMDB_API_KEY=your_tmdb_api_key
```

Replace `your_tmdb_api_key` with your actual API key from [TMDb](https://www.themoviedb.org/documentation/api).

### 4. Run the Application

```bash
npm run dev
```

Your app should now be running at `http://localhost:5173`.

---

## 🔌 API Reference

- **TMDb API Base URL**: `https://api.themoviedb.org/3`
- **Search Movies**: `/search/movie?query={query}`
- **Popular Movies**: `/discover/movie?sort_by=popularity.desc`

> Make sure you include the `Authorization` header using your TMDb Bearer token.

---

## 🧠 Backend (Appwrite)

This app uses Appwrite to:

- 📊 Track search analytics (`updateSearchCount`)
- 🔥 Fetch trending movies stored in the Appwrite database (`getTrendingMovies`)

You must configure your Appwrite SDK and database in `appwrite.js`.

---

## 🚀 Deployment

You can deploy this app using:

- [Netlify](https://www.netlify.com/)
- [Vercel](https://vercel.com/)
- [Render](https://render.com/)
- [GitHub Pages](https://pages.github.com/) (with build output)

Make sure to set your **VITE_TMDB_API_KEY** in the environment variables of the deployment platform.

---

## 💡 Future Improvements

- 🎭 Movie genres filter
- 🎬 Detailed movie modal popup
- 📲 Mobile-first UI enhancements
- 🧠 Personalized movie recommendations
- 🔒 User authentication (watchlist support)

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 💖 Acknowledgements

- [TMDb API](https://www.themoviedb.org/documentation/api)
- [React](https://react.dev/)
- [Appwrite](https://appwrite.io/)
- [react-use](https://github.com/streamich/react-use)

---

## 👨‍💻 Author

**Tushansh Bajaj**

- [Portfolio](https://tushanshbajaj.netlify.app/)
- [GitHub](https://github.com/Tushansh)
- [LinkedIn](https://www.linkedin.com/in/tushansh-bajaj-393169309)

---

> ⭐ Don’t forget to leave a star if you found this project helpful!