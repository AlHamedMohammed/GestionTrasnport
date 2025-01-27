# Data Analysis ML Application

This is a Flask-based desktop application for data analysis with machine learning capabilities.

---

## Development Setup Guide

### 1. Activate the Virtual Environment

First, navigate to the project directory:
```bash
cd /path/to/data_analysis_app
```

Then activate the virtual environment:
- On Linux/Mac:
 ```bash
 source venv/bin/activate
 ```
- On Windows:
 ```bash
 .\venv\Scripts\activate
 ```

You'll know it's activated when you see `(venv)` at the beginning of your terminal prompt.

---

### 2. Start the Flask Application

Once the virtual environment is activated, start the Flask application:
```bash
python app.py
```

The application will be available at: [http://localhost:5000](http://localhost:5000)

---

### 3. Development Workflow

- Make your code changes in your preferred editor.
- The Flask development server will automatically reload when you save changes.
- View the changes in your web browser at [http://localhost:5000](http://localhost:5000).
- Check the terminal for any error messages or logs.

---

### 4. Installing New Dependencies

If you need to install new Python packages:
```bash
pip install package_name
```

Don't forget to update `requirements.txt` after installing new packages:
```bash
pip freeze > requirements.txt
```

---

### 5. Deactivate the Virtual Environment

When you're done working, deactivate the virtual environment:
```bash
deactivate
```

---

## Project Structure

```
data_analysis_app/
|-- MLmodel.py               # ML model implementations
|-- database/                # Database related code
|   |-- db.py                # Database configuration
|   |-- __init__.py
|   |-- preprocess.py        # Preprocessing functions
|
|-- routes/                  # Application routes
|   |-- export_routes.py     # Export endpoints
|   |-- visualization_routes.py # Visualization endpoints
|
|-- visualization/           # Visualization code
|   |-- charts.py            # Chart generation
|   |-- visualisation.js     # Visualization functionality
|
|-- uploads/                 # Directory for uploaded files
|-- config.py                # Configuration settings
|-- README.md                # Project documentation
