IRCTC Train Information System
Description
The IRCTC Train Information System is a command-line Python application designed to interact with the Indian Railways API, allowing users to access various real-time train-related services. The application provides a user-friendly interface for checking live train status, PNR (Passenger Name Record) status, train schedules, live station status, and seat availability.

Features
Live Train Status: Check the real-time status of trains.
PNR Status: Verify the status of a PNR number.
Train Schedule: Retrieve detailed train schedules, including station names, arrival/departure times, and distances.
Live Station Status: See trains arriving or departing from a particular station in real-time.
Seat Availability: Check seat availability for specific journeys.
Technologies Used
Python: Core programming language used for the application.
Requests Library: Used to handle HTTP requests and interact with the Indian Railways API.
API Integration: Real-time data fetched from the Indian Railways API.
How to Use
Clone the Repository:
bash
Copy code
git clone https://github.com/yourusername/irctc-train-information-system.git
Install Required Libraries: Make sure you have requests installed:
bash
Copy code
pip install requests
Run the Application: After setting up, run the Python script:
bash
Copy code
python irctc_train_info.py
Choose from the Menu: The application will prompt you to choose one of the following options:
markdown
Copy code
1. Check live train status
2. Check PNR status
3. Check train schedule
4. Check live station status
5. Check seat availability
6. Exit
API Key Setup
To use the application, you need an API key from the Indian Railways API. Replace the placeholder api_key in the code with your actual API key:

python
Copy code
self.api_key = "your_api_key_here"
You can get the API key by signing up on Indian Railways API.

Example Usage
Checking Train Schedule: Enter the train number to retrieve the schedule:

less
Copy code
Enter train number: 12345
Output:
Station Name | Arrival Time | Departure Time | Distance (kms)
Checking PNR Status: Enter your 10-digit PNR number to get the status of your booking:

yaml
Copy code
Enter PNR number: 1234567890
Output:
PNR Status: Confirmed/Waiting List, etc.
Error Handling
The application gracefully handles errors like invalid train numbers, PNR numbers, or network issues by showing appropriate messages to the user.
Outcome
This project demonstrates:

Integration with real-time APIs.
Use of Python for practical data handling.
Robust error handling and validation of JSON responses.
User-friendly command-line interface for retrieving important train information.
Future Enhancements
Adding support for more features such as fare inquiry and train cancellation notices.
Improving the user interface for better usability.
