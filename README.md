README.md for HNG Internship Python Project
md
Copy
Edit
# Number Classification API  

This is a Flask-based API that classifies numbers based on mathematical properties and provides a fun fact about the number.  

## 📌 Features  
- **Prime Number Detection**: Determines if a number is prime.  
- **Perfect Number Check**: Identifies whether a number is a perfect number.  
- **Armstrong Number Check**: Detects if a number is an Armstrong number.  
- **Odd/Even Classification**: Checks if a number is odd or even.  
- **Digit Sum Calculation**: Computes the sum of a number’s digits.  
- **Fun Fact**: Fetches a fun fact about the number from the Numbers API.  

## 🚀 Live API Endpoint  
https://hng-internship-python-project-2-production-574a.up.railway.app/api/classify-number

yaml
Copy
Edit

## 🔧 How to Use  
### **1️⃣ Make a GET Request**  
Use this format to classify a number:  
https://hng-internship-python-project-2-production-574a.up.railway.app/api/classify-number?number=5

bash
Copy
Edit

### **2️⃣ Example Response**  
```json
{
  "digit_sum": 5,
  "fun_fact": "5 is the number of Justices on the Supreme Court of the United States necessary to render a majority decision.",
  "is_perfect": false,
  "is_prime": true,
  "number": 5,
  "properties": [
    "armstrong",
    "odd"
  ]
}
3️⃣ Error Handling
If an invalid input is provided, the API returns a 400 Bad Request:
Example:

bash
Copy
Edit
https://hng-internship-python-project-2-production-574a.up.railway.app/api/classify-number?number=abc
Response:

json
Copy
Edit
{
  "number": "invalid",
  "error": true
}
🛠️ Installation & Running Locally
1️⃣ Clone the Repository
sh
Copy
Edit
git clone https://github.com/adenijifisayo/hng-internship-python-project-2.git
cd hng-internship-python-project-2
2️⃣ Install Dependencies
sh
Copy
Edit
pip install -r requirements.txt
3️⃣ Run the API
sh
Copy
Edit
python app.py
The API will be available at:

arduino
Copy
Edit
http://127.0.0.1:5000/api/classify-number?number=5
🛠️ Deployment
This API is deployed on Railway. The production link is:

bash
Copy
Edit
https://hng-internship-python-project-2-production-574a.up.railway.app/api/classify-number
📜 License
This project is open-source and available under the MIT License
