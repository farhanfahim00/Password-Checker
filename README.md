# 🔒 Secure Password Checker  

This is a **Python-based password security tool** that checks whether a given password has been exposed in past data breaches using the **Have I Been Pwned API**.  

## 🚀 Features  
✔ Uses **SHA-1 hashing** to keep passwords secure  
✔ Leverages **Have I Been Pwned API** without exposing full passwords  
✔ Provides **real-time results** on password security  
✔ Helps users avoid using compromised passwords  

## 📌 How It Works  
1. The password is **hashed using SHA-1** encryption.  
2. The **first 5 characters** of the hash are sent to the API.  
3. The API returns a list of potential password hashes.  
4. The script checks if the full hash exists in the database.  
5. If found, it informs the user how many times the password has been leaked.

## ⚠️ Security Note  
This tool never sends your full password to an external server, ensuring privacy and security.

## 🛠 Installation & Usage 
### 🔧 Prerequisites  
- Python 3.x  
- `requests` library (install using `pip install requests`)  

### ▶ Running the Script  
```bash
python password_checker.py yourpassword123

#Example Output

Your Password: (yourpassword123) was FOUND 5000 times.. you should change it 

