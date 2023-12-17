
# nama aplikasi

Deskrpsi applikasi

## How to Run

1. Setelah clone projek dan membukanya
2. Buat Database dengan nama db_employee
3. Sesuaikan config database anda di app.py
    ```bash
      app.config['SQLALCHEMY_DATABASE_URI'] = 'postgresql://username:password@localhost/db_employee'
    ```

4. Install Python 3

   [Download python](https://www.python.org/downloads/0)


5. Install Virtual Environment

    ```bash
    Set-ExecutionPolicy Unrestricted -Scope Process
    pip3 install virtualenv
    ```

6. Create Virtual Environment di path ini

    ```bash
    python -m venv venv
    ```


7. Aktifasikan Virtual Environment

    ```bash
    venv\Scripts\activate
    ```

    Nonaktifkan
    ```bash
    deactivate
    ```

8. Install requirement dengan command:
    ```bash
    pip install -r requirements.txt
    ```
    
9. Makemigrations Database
    ```bash
    flask db stamp head
    flask db migrate -m 'your descriptive message'
    flask db upgrade
    ```
    
10. Jalan kan server
    ```bash
    flask run
    ```