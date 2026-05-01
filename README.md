# 🔐 API Security Risk Assessment (SaaS-Oriented Project)

## 📌 Overview
This project demonstrates a read-only API security assessment performed on a public REST API.

The goal was to identify common API security risks such as:
- Missing authentication
- Excessive data exposure
- Lack of access control
- Potential abuse scenarios

---

## 🎯 Target API
- https://jsonplaceholder.typicode.com

---

## 🛠️ Tools Used
- Postman
- Browser DevTools
- Kali Linux
- GitHub

---

## 🔍 Key Findings

### Missing Authentication (High)
API endpoints are accessible without login.

### Excessive Data Exposure (Medium)
User data such as email, phone, and address is exposed.

### Email Exposure (Medium)
Comments API reveals email addresses.

### ID-Based Access (Medium)
User data accessible via `/users/1`.

### No Rate Limiting (Low)
No visible request limits.

---

## 📸 Evidence

- users_endpoint.png  
- comments_exposure.png  
- user_id_access.png  
- postman_request.png  

---

## 📊 Impact

- Unauthorized data access  
- Privacy risks  
- Data scraping  
- Phishing possibilities  

---

## 🛡️ Recommendations

- Add authentication  
- Limit sensitive data  
- Implement access control  
- Apply rate limiting  

---

## 📄 Report
See: **report.pdf**

---

## ⚠️ Disclaimer
This project uses a public test API. No real systems were harmed.

---

## 👤 Author
Tushar Kunwar
