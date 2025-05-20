
# 🏥 Hospital Management System

A web-based Hospital Management System built using **Python**, **Django**, and **MongoDB**, designed to manage hospital operations including patients, doctors, appointments, medical records, and billing.

---

## 🔧 Features

* 👨‍⚕️ User Roles: Admin, Doctor, Receptionist, Patient
* 🗓️ Appointment Scheduling and Management
* 📋 Electronic Medical Records (EMR)
* 💊 Prescription Management
* 💵 Billing & Invoices
* 📊 Dashboard for analytics and reporting
* 🔐 Role-based access control
* 🔎 Search and filter patients, doctors, records

---

## 🛠️ Tech Stack

* **Backend:** Python 3, Django
* **Database:** MongoDB (via Djongo or PyMongo)
* **Frontend:** HTML5, CSS3, Bootstrap, JavaScript
* **Others:** Django Admin, Django Forms, Django ORM

---

## 🧰 Requirements

* Python 3.x
* MongoDB Server (local or cloud like MongoDB Atlas)
* `djongo` or `pymongo` (depending on integration method)
* Virtualenv (recommended)

---

## 🚀 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/hospital-management-system.git
   cd hospital-management-system
   ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure MongoDB**

   * Make sure MongoDB is running.
   * Update your `settings.py`:

     ```python
     DATABASES = {
         'default': {
             'ENGINE': 'djongo',
             'NAME': 'hospital_db',
         }
     }
     ```
   * Or, if using PyMongo manually, handle DB logic using `pymongo`.

5. **Apply initial migrations**

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create a superuser**

   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server**

   ```bash
   python manage.py runserver
   ```

8. Open in browser: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## 🧪 Example User Roles

| Role         | Permissions                                |
| ------------ | ------------------------------------------ |
| Admin        | Full control over all modules              |
| Doctor       | View schedule, update records, write notes |
| Receptionist | Register patients, schedule appointments   |
| Patient      | View personal records and appointments     |

---

## 📁 Project Structure

```
hospital_management/
├── hospital/            # Core logic (appointments, billing)
├── users/               # Authentication and role management
├── templates/           # HTML templates
├── static/              # Static files
├── manage.py
├── settings.py
├── requirements.txt
```

---

## 📦 Requirements (`requirements.txt`)

```txt
Django>=4.0
djongo>=1.3
pymongo>=4.0
djangorestframework
bootstrap4
```

---

## ✅ Future Enhancements

* REST API for mobile clients
* Appointment reminders via email/SMS
* Role-based dashboards with charts
* Payment gateway integration

---

## 📄 License

This project is licensed under the MIT License.

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests.

---


