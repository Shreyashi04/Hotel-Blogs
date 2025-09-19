# 📘 EROOMS - Your Room, Your Choice

**EROOMS** is a fully functional Django-based web application for listing and browsing rental rooms with key details like address, host info, and user reviews. The platform features dark mode, profile picture support, search functionality, and smooth navigation for a better user experience.

---


## 🚀 Features
- 🔒 **User Authentication:** Register, Login, Logout  
- 👤 **Profile Management:** Edit profile with image  
- 🏡 **Room Listings:** Browse all available rooms  
- 🔍 **Search Bar:** Search by title or address  
- 🌓 **Dark Mode Toggle:** Smooth UI toggle with local storage  
- 🗺️ **Listing Page:** Address, photos, and review details  
- ⭐ **Rating System:** User reviews with star ratings  
- 📱 **Responsive Design:** Mobile and desktop friendly  
- 🧭 **Pagination:** Better experience for large listing datasets  

---

## 🧰 Tech Stack

| Layer      | Technology                  |
|------------|----------------------------|
| Language   | Python 3.9+                |
| Framework  | Django 4.x                 |
| Database   | SQLite3 (default)          |
| Frontend   | HTML5, CSS3                |
| Templating | Django Templates           |
| Static Files | Custom CSS & SVG          |
| Hosting    | (Your deployment provider here) |

---

## 📷 Screenshots
*(Add screenshots here, for example)*  
- Home Page with Listings  
- Listing Details with Reviews  
- User Profile with Picture  
- Dark Mode UI  

---

## ⚙️ Getting Started

1.Clone the Repository
```
git clone https://github.com/your-username/Hotel-Blogs.git
cd erooms
```
2.Create Virtual Environment
```
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
```

3.Run Migrations
```
python manage.py migrate
```

4.Create Superuser (Admin)
```
python manage.py createsuperuser
```

5.Start the Server
```
python manage.py runserver
```

6.Visit:
```
http://127.0.0.1:8000/
```
---
## 🔗 Available URLs

| Path             | Purpose               |
| ---------------- | --------------------- |
| `/`              | Home page (Listings)  |
| `/login/`        | Login user            |
| `/register/`     | Register new user     |
| `/profile/<id>/` | View user profile     |
| `/editprofile/`  | Edit profile          |
| `/logout/`       | Logout user           |
| `/listing/<id>/` | Detailed listing page |

---

## 🧬 Models Overview

- User – Django's built-in auth.User

- Profile (authy.models.Profile)
  - user (OneToOneField)
  - image
  - bio / details

- Listing (post.models.Listing)
  title, address, photos, owner

- Photo (post.models.Photo)
  ForeignKey to Listing

- Review (post.models.Review)
  - rating, comment
  - ForeignKey to Listing and User

---
## 📜 License  

This project is licensed under the **MIT License**.  

