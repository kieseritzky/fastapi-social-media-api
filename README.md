# Social Media API build with FastAPI

A social media api that allows users to login, post and vote on other posts. 

The project has the following features:

## 🚀 Features

* **JWT Authentication**: It allows users to login with their credentials and ensures safety of other users data.
* **Alembic Revisions**: It uses alembic revisions to upgrade and downgrade safely.
* **SQLAlchemy ORM**: It uses SQLAlchemy orm to talk efficiently to the postgres database.
* **Postgresql**: It stores the data in users, posts and votes tables in the postgresql database.
* **Voting System**: It features a voting system that allows users to vote and unvote on other users posts.


## 🛠️ Prerequisites & Installation
 
1. **Clone or navigate to the repository:**
   ```terminal
   git clone "copy the repo url here"
   cd "directory name here"
   ```
2. **Create a virtual environment:**
    ```terminal
    python -m venv venv
    venv/Scripts/activate

3. **Install Requirements:**
   ```terminal
   pip install -r requirements.txt
   ```

4. **Create .env file:**
    
   Open the folder in vs code or any other editor.
   Create a .env file.
   Add the Following:

   DATABASE_HOSTNAME=localhost
   DATABASE_PORT=5432
   DATABASE_USERNAME=yourdatabaseserverusername
   DATABASE_PASSWORD=yourdatabaseserverpassword
   DATABASE_NAME=databasenameofyourpostgresqldatabase
   SECRET_KEY=anyrandomlongstringofkeys
   ALGORITHM=HS256
   ACCESS_TOKEN_EXPIRE_MINUTES=30

   
5. **Run migrations:**
In your ide terminal:
   ```terminal
   alembic upgrade head
   
   ```
## 💻 How to Run

Execute the main script from your ide terminal:
```terminal
uvicorn app.main:app --reload
```

Go to 127.0.0.1:8000/docs in your browser

## License

This project is licensed under the MIT License.
