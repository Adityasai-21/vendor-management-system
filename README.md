# vendor-management-system
A Vendor Management System (VMS) is a comprehensive platform designed to streamline and automate the process of managing vendor relationships. It serves as a centralized hub for businesses to efficiently oversee various aspects of vendor interactions, including vendor selection, onboarding, performance monitoring, and payment processing.




INITIAL SETUP

Clone the repository:
git clone https://github.com/Adityasai-21/vendor-management-system

Navigate to the project directory:
cd Vendor-management-system

Activate virtualenv
venv\scripts\activate


Install dependencies:
pip install -r requirements.txt


Apply database migrations:
python manage.py migrate


Run the development server using following command:
python manage.py runserver

----------------------------------------------
Setup instructions and details on using the API endpoints:

I have used Postman for API testing and demonstrated the functionality and reliability of the endpoints.

Follow the url below and click on 'Run in Postman' which is in the top right side corner to open Postman


API test suite - https://documenter.getpostman.com/view/31500665/2s9YeLZpj5


-----------------------------------------------------------------------------

API Endpoint Details:


VENDORS:

1. List/Create Vendors:

URL: api/vendors/
Method: GET (List Vendors), POST (Create Vendor)
Authentication: Token Authentication required

2. Retrieve/Update Vendor:

URL: api/vendors/<int:pk>/
Method: GET (Retrieve Vendor), PUT (Update Vendor)
Authentication: Token Authentication required

3. Delete Vendor:

URL: api/vendors/delete/<int:pk>/
Method: DELETE
Authentication: Token Authentication required

PURCHASE ORDERS:

1. List/Create Purchase Orders:

URL: api/purchase-orders/
Method: GET (List Purchase Orders), POST (Create Purchase Order)
Authentication: Token Authentication required

2. Retrieve/Update Purchase Order:

URL: api/purchase-orders/<int:pk>/
Method: GET (Retrieve Purchase Order), PUT (Update Purchase Order)
Authentication: Token Authentication required

3. Delete Purchase Order:

URL: api/purchase-orders/delete/<int:pk>/
Method: DELETE
Authentication: Token Authentication required.

--------------------------------------------

Acknowledge Purchase Order:

URL: api/purchase-orders/<int:pk>/acknowledge/
Method: PUT (Acknowledge Purchase Order)
Authentication: Token Authentication required


Retrieve Vendor Performance:

URL: /vendors/<int:pk>/performance/
Method: GET (Retrieve Vendor Performance)
Authentication: Token Authentication required


