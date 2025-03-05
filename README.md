# URL Shortener 

This project is built with Django, Bootstrap, and SweetAlert2. It allows users to input a long URL and receive a shortened version using the `pyshorteners` library.

## Features

-   **URL Shortening:** Converts long URLs into shorter, more manageable links.
-   **User-Friendly Interface:** Uses Bootstrap for a responsive and clean design.
-   **Error Handling:** Provides clear error messages for invalid URLs.
-   **Copy to Clipboard:** Allows users to easily copy the shortened URL.
-   **SweetAlert2 Integration:** Displays success and error messages using stylish pop-ups.

## Requirements

-   `pyshorteners` 
-   `asgiref`
-   `certifi`
-   `charset-normalizer`
-   `idna`
-   `pyperclip`
-   `requests`
-   `sqlparse`
-   `tzdata`
-   `urllib3`

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/Vedant-Raulkar/Url-Shortener
    cd Url-Shortener
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS and Linux
    venv\Scripts\activate  # On Windows
    ```

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Apply migrations:**

    ```bash
    python manage.py migrate
    ```

5.  **Run the development server:**

    ```bash
    python manage.py runserver
    ```

6.  **Open your browser and navigate to `http://127.0.0.1:8000/`**

## Usage

1.  Enter the URL you want to shorten in the input field.
2.  Click the "Submit" button.
3.  If the URL is valid, a SweetAlert2 pop-up will display the shortened URL with a "Copy" button.
4.  If the URL is invalid, an error message will be displayed.
5.  You can copy the shortened URL to your clipboard by clicking the "Copy" button.

## Project Structure

url-shortener/
├── urlshortener/
│   ├── init.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   ├── views.py
│   ├── forms.py
├── manage.py
├── templates/
│   └── home.html
├── requirements.txt


- `urlshortener/views.py`: Contains the logic for URL shortening and rendering the form.
- `urlshortener/forms.py`: Defines the form for URL input.
- `templates/home.html`: The HTML template for the URL shortener page.
- `requirements.txt`: Lists the project's dependencies.

## Dependencies

-   **Django:** Web framework for building the application.
-   **Bootstrap:** CSS framework for styling the user interface.
-   **SweetAlert2:** JavaScript library for displaying beautiful and responsive alerts.
-   **pyshorteners:** Python library for shortening URLs.
-   **Clipboard.js:** JavaScript library to copy text to the clipboard.

