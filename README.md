# Flask Message Board

A simple message board web app built with **Flask** and SQLite — inspired by the [Real Python Flask tutorials](https://realpython.com/).

---

## Features

- Post and view messages
- Uses Flask Blueprints for clean project structure
- Stores posts in a SQLite database
- Uses environment variables with `python-dotenv`
- Includes static CSS and Jinja2 templates

---

## Tech Stack

- Python 3.x
- Flask
- SQLite
- Click (for CLI commands)
- python-dotenv

---

## Getting Started

Follow these steps to run the project locally on your Mac.

1. Clone the Repository

```
bash
git clone https://github.com/achinta726/rp_flask_board.git
cd rp_flask_board
```

2. Create & Activate a Virtual Environment 
```
python3 -m venv venv  
source venv/bin/activate  # for macOS/Linux
```
 For Windows:  
``` 
venv\Scripts\activate
```

3. Install Dependencies
```
pip install -r requirements.txt
```

5. Create a .env file 
At the project root, create a .env file:

```
ENVIRONMENT=Development  
SECRET_KEY=your-secret-key  
DATABASE_URL=sqlite:///board.sqlite
```

5. Initialize the Database 
```
flask --app board init-db
```

7. Run the Application  
```
flask --app board run --port 8000 --debug
```

Open http://127.0.0.1:8000 in your browser.  

Project Structure

```
rp_flask_board/  
├── board/  
│   ├── __init__.py  
│   ├── posts.py  
│   ├── templates/  
│   │   ├── base.html  
│   │   └── posts/  
│   │       └── create.html  
│   ├── static/  
│   │   └── styles.css  
│   └── db.py  
├── venv/  
├── .env  
├── .gitignore  
├── requirements.txt  
├── README.md

```
