# cafe_wifi

## Café & Wifi — Find the Perfect Café to Sip, Work, and Connect

A Flask‑based web application that helps users discover cafés with reliable Wi‑Fi, comfortable seating, power outlets, and essential amenities.
Browse cafés, view photos, check details, create an account, log in, and add new café locations. **


## ✨ Features
- Browse cafés with photos and detailed information

- View café location via Google Maps

- Check amenities:

- Wi‑Fi availability

- Power sockets

- Toilet access

- Seating

- Phone‑friendly environment

- User authentication (register, login, logout)

- Add new cafés (members only)

- Secure password hashing (bcrypt)

- CSRF protection (Flask‑WTF)

- SQLite database for easy local development

## 🗂 Project Structure

cafe_wifi/
│
├── cafeteria/
│   ├── __init__.py
│   ├── routes.py
│   ├── models.py
│   ├── forms.py
│   └── static/
│       └── images/
│
├── templates/
│   ├── home.html
│   ├── login.html
│   ├── register.html
│   ├── cafes.html
│   └── add_cafe.html
│
├── cafes.db
├── run.py
├── requirements.txt
└── README.md


## 🚀 Getting Started

### 1. Clone the repository
Code
git clone https://github.com/RamsesPH/cafe_wifi.git
cd cafe_wifi

### 2. Create a virtual environment (Python 3.9 recommended)

pyenv local 3.9.18
python -m venv venv
source venv/bin/activate

### 3. Install dependencies

pip install -r requirements.txt

### 4. Create a .env file

SECRET_KEY=your_secret_key_here
API_KEY=your_google_maps_api_key

### 5. Run the application

python run.py

## 🧠 How It Works
Users browse cafés stored in cafes.db

Each café includes:

- Name

- Location

- Google Maps link

- Amenities

- Photo

- Registered users can add new cafés

- Passwords are hashed using bcrypt

- CSRF protection is enabled for all forms

## 📌 Known Issues

- Some café photos may not display if:

- The file is missing from /static/images/

- The filename in the database does not match

- The path in the template is incorrect

- The image URL is broken

- Use Fix missing café photos to resolve

## 📄 License

This project is open‑source and available under the MIT License.