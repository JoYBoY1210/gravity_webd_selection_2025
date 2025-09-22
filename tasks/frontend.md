# Frontend Tasks 🎨

Complete all three frontend tasks to demonstrate your web development skills.

---

## Task 1: Responsive Card Layout (15 points)

### Objective
Create a responsive grid layout displaying 4-6 profile cards.

### Requirements
- **Design**: Clean, professional appearance
- **Content**: Each card should include:
  - Profile photo/avatar
  - Name
  - Job role/title
  - Brief description (optional)
- **Responsiveness**: 
  - Desktop: 3-4 cards per row
  - Tablet: 2 cards per row
  - Mobile: 1 card per row
- **Styling**: Use CSS Grid or Flexbox
- **Hover Effects**: Add subtle animations

### Evaluation Criteria
- Code quality and organization (5 pts)
- Responsive design implementation (5 pts)
- Visual design and aesthetics (5 pts)

### Technologies
- HTML5
- CSS3 (Grid/Flexbox)
- Optional: CSS preprocessors (SASS/LESS)

---

## Task 2: Signup/Login Form with Validation (20 points)

### Objective
Build an interactive form with real-time validation.

### Requirements
- **Form Fields**:
  - Email (with email format validation)
  - Password (minimum 8 characters, at least 1 number, 1 special character)
  - Confirm Password (must match password)
- **Validation**:
  - Real-time validation on input
  - Visual feedback (error/success states)
  - Prevent form submission if validation fails
- **UX Features**:
  - Toggle password visibility
  - Clear error messages
  - Smooth animations

### Evaluation Criteria
- Form validation logic (8 pts)
- User experience and design (7 pts)
- Code structure and best practices (5 pts)

### Technologies
- HTML5
- CSS3
- Vanilla JavaScript (DOM manipulation)

---

## Task 3: GitHub Profile Fetcher (30 points)

### Objective
Create an application that fetches and displays GitHub user information.

### Requirements
- **Input**: Text field for GitHub username
- **Output Display**:
  - User avatar
  - Full name
  - Username
  - Bio/description
  - Number of public repositories
  - Followers/Following count
- **Error Handling**:
  - Handle invalid usernames
  - Network error handling
  - User-friendly error messages
- **Features**:
  - Loading state while fetching
  - Search history (bonus)
  - Responsive design

### API Endpoint
```
GET https://api.github.com/users/{username}
```

### Evaluation Criteria
- API integration and error handling (12 pts)
- UI/UX design and responsiveness (10 pts)
- Code quality and organization (8 pts)

### Technologies
- HTML5, CSS3, JavaScript
- Fetch API or Axios
- Optional: Local Storage for search history

---

## Submission Guidelines

1. Create a folder: `frontend/` in your submission directory
2. Organize tasks in subfolders:
   ```
   frontend/
   ├── task1-cards/
   │   ├── index.html
   │   ├── style.css
   │   └── README.md
   ├── task2-forms/
   │   ├── index.html
   │   ├── style.css
   │   ├── script.js
   │   └── README.md
   └── task3-github-fetcher/
       ├── index.html
       ├── style.css
       ├── script.js
       └── README.md
   ```
3. Include a README.md for each task explaining:
   - How to run the project
   - Features implemented
   - Any additional libraries used

## Tips for Success 💡

- **Mobile-First**: Start with mobile design, then scale up
- **Accessibility**: Use semantic HTML and proper ARIA labels
- **Performance**: Optimize images and minimize HTTP requests
- **Browser Testing**: Test on multiple browsers
- **Code Comments**: Document your code for better readability

**Good luck! 🚀**
