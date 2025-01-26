# Blog API

This project is a RESTful API for managing blog posts and comments. It is built using **Django** and **Django REST Framework (DRF)**. The API supports creating, reading, updating, and deleting (CRUD) blog posts and comments. It can be extended to include authentication and additional features like search, filtering, algorithmic recomendation and other commonly found features in blogging system.

---

## Features

- CRUD operations for blog posts and comments
- Nested comments linked to their respective blog posts
- JSON responses for easy integration with frontend applications
- Scalable and extensible structure

---

## Technologies Used

- **Python 3.8+**
- **Django 4.x**
- **Django REST Framework**
- **SQLite (default, replaceable with other databases)**

---

## Installation

### Prerequisites

- Python installed on your system
- `pip` package manager
- (Optional) Virtual environment tool like `venv`

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/QTDevi/API_Blog.git
   cd blog_project
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Dependencies**:
   ```bash
   pip install django djangorestframework
   ```

4. **Run Database Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Start the Development Server**:
   ```bash
   python manage.py runserver
   ```

6. **Access the API**:
   Visit `http://127.0.0.1:8000/api/` in your browser or use a tool like Postman.

---

## Endpoints

### Posts
- **GET** `/api/posts/`: Retrieve all posts
- **POST** `/api/posts/`: Create a new post
- **GET** `/api/posts/<id>/`: Retrieve a specific post
- **PUT** `/api/posts/<id>/`: Update a post
- **DELETE** `/api/posts/<id>/`: Delete a post

### Comments
- **GET** `/api/comments/`: Retrieve all comments
- **POST** `/api/comments/`: Create a new comment
- **GET** `/api/comments/<id>/`: Retrieve a specific comment
- **PUT** `/api/comments/<id>/`: Update a comment
- **DELETE** `/api/comments/<id>/`: Delete a comment

---

## File Structure

```
blog_project/
├── blog_project/
│   ├── settings.py        # Project settings
│   ├── urls.py            # Project-level URLs
│   ├── ...
├── blog/
│   ├── models.py          # Database models
│   ├── serializers.py     # DRF serializers
│   ├── views.py           # API views
│   ├── urls.py            # App-level URLs
│   ├── ...
├── manage.py              # Django CLI tool
```

---

## Future Improvement Plans

- **Authentication**: Add user authentication to secure the API.
- **Algorithm**: Add user interaction based algorithm.
- **Pagination**: Implement pagination for blog posts and comments.
- **Search and Filtering**: Allow filtering posts by title or content.
- **Deployment**: Use Docker and deploy on a cloud platform like AWS, or GCP. # Low Priority

---

## License

This project is licensed under no licence and is a template in progress.

