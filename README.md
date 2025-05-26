# 🤖 Vending Business Location Finder Assistant

**AI-powered intelligence for putting your vending machines where they’ll earn the most.** Built with cloud-native best practices, the app pairs geospatial search with GPT-4 copywriting to hand you both 📍 **high-traffic locations** and 💬 **tailored cold-call scripts**—all in seconds.

---

## ✨ Key Features

|                                 |                                                                                                                |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| 🔎 **Search by ZIP**            | Enter any U.S. ZIP code and instantly retrieve latitude/longitude coordinates.                                 |
| 🏷️ **Pick a Machine Type**     | Snacks, drinks, coffee, PPE—choose what you vend to refine venue matches.                                      |
| 📊 **AI-Ranked Venues**         | The Location Engine queries Google Maps and scores gyms, offices, schools, hotels & more for foot-traffic fit. |
| 📞 **Custom Cold-Call Scripts** | GPT-4 drafts a 30-second pitch plus objection-handling bullets matched to each venue persona.                  |
| 💻 **Modern UI**                | Responsive Bootstrap 5 front end with dynamic charts & toast notifications.                                    |
| ☁️ **Cloud-Native Stack**       | Container-ready Flask API, SQLAlchemy ORM, 12-factor configuration, CI-ready.                                  |

---

## 🚀 Quick Start

```bash
# 1 ▸ Clone
git clone https://github.com/your-handle/vending-location-finder.git
cd vending-location-finder

# 2 ▸ Virtual env
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# 3 ▸ Install deps
pip install -r requirements.txt

# 4 ▸ Environment vars
cp .env.example .env          # then add your keys ✍️
#   OPENAI_API_KEY=pk-…
#   GOOGLE_MAPS_API_KEY=AIza…

# 5 ▸ Run the app
python app.py                 # http://localhost:5000
```

---

## 🗂️ Project Structure

```
vending-location-finder/
├── app/                      # Flask application package
│   ├── __init__.py           # Factory + extensions
│   ├── models.py             # SQLAlchemy ORM models
│   ├── routes.py             # Blueprints / API routes
│   ├── services/             # Core business logic
│   │   ├── location_service.py
│   │   └── script_generator.py
│   └── templates/            # Jinja2 HTML templates
│       ├── base.html
│       ├── index.html
│       └── results.html
├── static/                   # Front-end assets
│   ├── css/style.css
│   └── js/main.js
├── requirements.txt          # Python dependencies
├── app.py                    # Entrypoint (for dev)
└── .env.example              # Sample environment file
```

---

## 🛠️ Tech Stack

| Layer      | Tech                                        |
| ---------- | ------------------------------------------- |
| Backend    | **Python 3 · Flask**                        |
| Data       | **SQLAlchemy** + SQLite/PostgreSQL          |
| AI         | **OpenAI GPT-4** for copy generation        |
| Geospatial | **Google Maps Places API**                  |
| Front-End  | **HTML5 · CSS3 · JavaScript · Bootstrap 5** |
| DevOps     | Docker-ready, .env config, GitHub CI        |

---

## 📈 Roadmap

* [ ] Docker Compose for one-command local spin-up
* [ ] Swagger / OpenAPI 3 docs
* [ ] OAuth so multiple reps can save venue short-lists
* [ ] Automated unit + integration test suite in CI
* [ ] Deploy-to-AWS (ECS + RDS) action

---

## 🤝 Contributing

1. **Fork** the repo
2. Create your feature branch (`git checkout -b feat/amazing‐idea`)
3. Commit your changes (`git commit -m 'feat: add amazing idea'`)
4. Push to the branch (`git push origin feat/amazing‐idea`)
5. Open a **Pull Request**

All PRs require a green test suite and follow Conventional Commits.

---

## 📝 License

Released under the **MIT License**. See [`LICENSE`](LICENSE) for details.

---

> *“Right machine, right place, right pitch—automated.”*
> **— Vending Business Location Finder Assistant**
