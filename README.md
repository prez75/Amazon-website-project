# Amazon-website-project

A functional web prototype: users register, log in, pick a role (student / parent / educator), and see T-Level information tailored to that role. Includes accessibility settings (dark mode, larger text, high contrast) and a contact/feedback form.

Academic / trademark disclaimer This is a student prototype built for an educational exercise. The "Amazon" name and styling are used only to resemble the brief. It is not affiliated with or endorsed by Amazon. Do not deploy publicly or present it as a real Amazon product.

Tech stack
Front end: HTML, CSS, vanilla JavaScript
Back end: Python + Flask
Database: SQLite (created automatically on first run)
Folder structure
amazon_student/
├── app.py                  # Flask app: routes, auth, validation, DB setup
├── requirements.txt        # Python dependencies
├── database.db             # SQLite DB (auto-created; git-ignored)
├── README.md
├── ASSETS_LOG.md           # Sources for code + content
├── .gitignore
├── static/
│   ├── css/
│   │   └── style.css       # All styling + theming (dark/contrast/large text)
│   └── js/
│       └── main.js         # Accessibility toggles, saved in localStorage
└── templates/
    ├── base.html           # Shared layout every page extends
    ├── home.html           # 1. Home
    ├── register.html       # 2. Register
    ├── login.html          # 3. Login
    ├── dashboard.html      # 4. Dashboard (routes by role)
    ├── student_info.html   # 5. Student information
    ├── parent_info.html    # 6. Parent information
    ├── educator_info.html  # 7. Educator information
    ├── settings.html       # 8. Settings (accessibility)
    └── contact.html        # 9. Contact us
