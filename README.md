# Vending Business Location Finder Assistant

An AI-powered tool that helps vending machine business owners find optimal locations for their machines and generate tailored cold-call scripts.

## Features

- Location search by zip code
- Vending machine type selection
- AI-powered location suggestions
- Customized cold-call script generation
- Modern, responsive user interface

## Setup

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file with your API keys:
   ```
   OPENAI_API_KEY=your_openai_api_key
   GOOGLE_MAPS_API_KEY=your_google_maps_api_key
   ```
5. Run the application:
   ```bash
   python app.py
   ```

## Project Structure

```
vending-location-finder/
├── app/
│   ├── __init__.py
│   ├── models.py
│   ├── routes.py
│   ├── services/
│   │   ├── __init__.py
│   │   ├── location_service.py
│   │   └── script_generator.py
│   └── templates/
│       ├── base.html
│       ├── index.html
│       └── results.html
├── static/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── main.js
├── .env
├── .gitignore
├── app.py
└── requirements.txt
```

## Technologies Used

- Python/Flask
- SQLAlchemy
- OpenAI API
- Google Maps API
- HTML5/CSS3
- JavaScript
- Bootstrap 5

## License

MIT License 