<h1 align="center">Hi 👋, I'm Sneha Sahu</h1>
<h3 align="center">🚀 Python Developer | ERPNext | Backend Developer</h3>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=snehasahu1798&label=Profile%20views&color=0e75b6&style=flat" alt="profile views" />
</p>

---

## 👩‍💻 About Me

- 💻 Python Developer with hands-on experience in **ERPNext & Frappe Framework**
- 🏢 Specialized in building and customizing **ERP solutions**
- 🔄 Experienced in **Workflow Automation & Backend Logic Development**
- 📊 Skilled in creating **Script Reports & Query Reports**
- 🛠 Passionate about solving real-world business problems through automation

---

## 🚀 ERPNext & Frappe Expertise

✔️ Custom DocType Development  
✔️ Client Scripts & Server Scripts  
✔️ Workflow Automation  
✔️ Custom ERP Modules  
✔️ REST API Integrations  
✔️ Role & Permission Management  
✔️ ERPNext Deployment & Setup  
✔️ Background Jobs & Scheduler Events  

---

## 🧠 Sample ERPNext Server Script

```python
import frappe

@frappe.whitelist()
def create_customer(name, email):
    customer = frappe.get_doc({
        "doctype": "Customer",
        "customer_name": name,
        "email_id": email
    })
    customer.insert(ignore_permissions=True)
    frappe.db.commit()
    return "Customer Created Successfully"
