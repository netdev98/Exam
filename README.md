Here’s a **README.md template** you can include in your GitHub repository for Exercise #2. It explains how to build, run, and test the solution, plus notes about assumptions and requirements.

---

# UserForm Component – Blazor Exercise

## 📌 Overview
This project contains a **reusable Blazor form component** (`UserForm.razor`) that collects user information (Name, Address, Age, Email). It demonstrates:
- Proper use of **EditForm** and Blazor input components.
- Validation with **DataAnnotations**.
- A reusable design with **parameters** and **EventCallback**.
- Support for **Create/Edit modes** without mutating parent data.
- An **async uniqueness check** for email.
- At least one field implemented with **manual binding** (Email).
- Clean, styled UI suitable for business applications.

---

## ⚙️ Project Structure
```
/Components
    UserForm.razor
/Pages
    UserFormDemo.razor
/wwwroot/css
    UserForm.css
README.md
```

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/blazor-userform.git
cd blazor-userform
```

### 2. Build the Project
```bash
dotnet build
```

### 3. Run the Application
```bash
dotnet run
```

### 4. Navigate to the Demo Page
Open your browser and go to:
```
https://localhost:5001/userformdemo
```

---

## 🧩 Usage

### Component (`UserForm.razor`)
- Accepts a `UserModel` from the parent.
- Exposes an `OnSubmit` event via `EventCallback<UserModel>`.
- Displays validation messages for each field.
- Prevents duplicate submissions with a disabled button state.
- Performs an async uniqueness check for email.

### Parent Page (`UserFormDemo.razor`)
- Instantiates a `UserModel`.
- Passes it into the component.
- Handles submitted data and displays it below the form.

---

## 🎨 Styling
The form uses `UserForm.css` for a clean, card-style layout:
- Consistent spacing and alignment.
- Styled buttons with hover effects.
- Validation messages in red.
- Success messages in green.

---

## 📋 Assumptions
- Email uniqueness check is mocked (`test@example.com` is considered taken).
- Business logic (e.g., saving to a database) is handled in the parent page.
- The component is designed for **Blazor Server or WebAssembly**.

---

## ✅ Requirements Met
- Reusable component with parameters and EventCallback.
- Proper Blazor fundamentals (`EditForm`, inputs, validation).
- Manual binding for Email field.
- Async uniqueness check.
- Create/Edit mode support.
- Clean UI and usability improvements.
- Clear project structure and instructions.

---

## 🎥 Feedback Video (to be added)
When submitting, include a short video (max 5 minutes) explaining:
1. How long it took to complete.  
2. Which part was easiest and why.  
3. One challenge and how you solved it.  
4. Why/how you used AI, if applicable.  

---

👉 This README ensures reviewers can **clone, build, run, and test** your solution with minimal effort.  

Would you like me to also prepare a **short sample transcript** for your feedback video (covering the 4 required points), so you’ll have a ready script to record?
