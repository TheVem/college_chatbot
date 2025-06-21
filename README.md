# College Chatbot

A Django-based chatbot application designed to help college students with frequently asked questions and provide automated responses.

## Features

- **FAQ Management**: Store and manage frequently asked questions and their answers
- **User Query Tracking**: Track user interactions and bot responses
- **Web Interface**: Clean and responsive chat interface
- **Admin Panel**: Django admin interface for managing FAQs and user queries

## Models

### FAQ
- `question`: The frequently asked question (max 500 characters)
- `answer`: The corresponding answer (text field)

### UserQuery
- `user_input`: The user's input message (max 500 characters)
- `bot_response`: The bot's response (text field)
- `timestamp`: When the query was made (auto-generated)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/TheVem/college_chatbot.git
cd college_chatbot
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run migrations:
```bash
python manage.py migrate
```

4. Create a superuser (optional):
```bash
python manage.py createsuperuser
```

5. Run the development server:
```bash
python manage.py runserver
```

## Usage

1. Access the chatbot at `http://localhost:8000/chatbot/`
2. Start chatting with the bot
3. Access the admin panel at `http://localhost:8000/admin/` to manage FAQs

## Project Structure

```
college_chatbot/
├── chatbot/                 # Main Django app
│   ├── models.py           # Database models
│   ├── views.py            # View logic
│   ├── urls.py             # URL routing
│   ├── templates/          # HTML templates
│   ├── static/             # Static files (CSS, JS)
│   └── data/               # Custom dataset
├── college_chatbot/        # Django project settings
│   ├── settings.py         # Project settings
│   └── urls.py             # Main URL configuration
└── manage.py               # Django management script
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE). 