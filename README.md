# ✅ My Tasks - Modern To-Do List App

<div align="center">

![To-Do List App](https://img.shields.io/badge/React-18.x-blue?style=for-the-badge&logo=react)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.x-38B2AC?style=for-the-badge&logo=tailwind-css)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

A beautiful, minimalist to-do list application built with React and Tailwind CSS featuring a peaceful color palette and smooth animations.

[Live Demo](#) • [Features](#features) • [Installation](#installation) • [Usage](#usage)

</div>

---

## 🌟 Features

- **✨ Beautiful UI/UX** - Peaceful teal and mint color palette with smooth animations
- **📝 Task Management** - Add, complete, and delete tasks with ease
- **🔍 Smart Filtering** - View all tasks, active tasks, or completed tasks
- **📊 Real-time Stats** - Track total, active, and completed tasks at a glance
- **💾 Local Storage** - Tasks persist across browser sessions
- **🎯 Keyboard Support** - Press Enter to quickly add tasks
- **🎨 Toast Notifications** - Visual feedback for all actions
- **📱 Responsive Design** - Works seamlessly on desktop, tablet, and mobile
- **🌙 Dark Mode Ready** - Full dark mode support (toggle coming soon)

## 🎨 Design System

- **Color Palette**: Soft teal (#4BA39A) with mint accents
- **Typography**: Inter for body text, Space Grotesk for headings
- **Components**: Built with shadcn/ui for accessibility
- **Animations**: Smooth transitions with cubic-bezier easing

## 🖼️ Screenshots

### Empty State
<img src="screenshots/empty-state.png" alt="Empty State" width="600">

### Active Tasks
<img src="screenshots/with-tasks.png" alt="With Tasks" width="600">

### Completed Tasks
<img src="screenshots/completed.png" alt="Completed Tasks" width="600">

## 🚀 Quick Start

### Prerequisites

- Node.js 16.x or higher
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/todo-list-app.git
   cd todo-list-app
   ```

2. **Install dependencies**
   ```bash
   cd frontend
   yarn install
   # or
   npm install
   ```

3. **Start the development server**
   ```bash
   yarn start
   # or
   npm start
   ```

4. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📖 Usage

### Adding a Task
1. Type your task in the input field
2. Click the "Add" button or press Enter
3. Your task will appear at the top of the list

### Completing a Task
1. Click the circle icon next to a task
2. The task will be marked with a checkmark and strikethrough
3. Stats will update automatically

### Deleting a Task
1. Click the trash icon on the right side of any task
2. The task will be removed immediately

### Filtering Tasks
1. Use the "All", "Active", or "Completed" buttons
2. The list will update to show only matching tasks

### Clearing Completed Tasks
1. Complete at least one task
2. Click "Clear Completed" button
3. All completed tasks will be removed at once

## 🛠️ Built With

### Frontend
- **React 18** - UI library
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - Re-usable component library
- **Lucide React** - Icon library
- **Sonner** - Toast notifications

### Development Tools
- **Create React App** - Project setup
- **ESLint** - Code linting
- **Prettier** - Code formatting

## 📁 Project Structure

```
todo-list-app/
├── frontend/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/              # shadcn/ui components
│   │   │   └── TodoApp.jsx      # Main todo component
│   │   ├── App.js               # App entry point
│   │   ├── App.css              # Custom animations
│   │   ├── index.css            # Design system tokens
│   │   └── index.js             # React entry point
│   ├── package.json
│   └── tailwind.config.js       # Tailwind configuration
└── README.md
```

## 🎯 Key Components

### TodoApp Component
The main component that handles all task management logic:
- State management with React hooks
- LocalStorage integration
- Task filtering logic
- Toast notifications

### Design System
Custom CSS variables in `index.css`:
- Color tokens (primary, secondary, accent)
- Gradients and shadows
- Animation timing functions
- Responsive breakpoints

## 💡 Technical Highlights

### LocalStorage Persistence
```javascript
// Save tasks automatically
useEffect(() => {
  localStorage.setItem('todoTasks', JSON.stringify(tasks));
}, [tasks]);

// Load tasks on mount
useEffect(() => {
  const savedTasks = localStorage.getItem('todoTasks');
  if (savedTasks) {
    setTasks(JSON.parse(savedTasks));
  }
}, []);
```

### Token-Based Design System
```css
:root {
  --primary: 174 45% 48%;  /* Soft Teal */
  --gradient-primary: linear-gradient(135deg, hsl(174 45% 48%), hsl(174 55% 58%));
  --transition-smooth: 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}
```

## 🔮 Future Enhancements

- [ ] Dark mode toggle
- [ ] Task priorities (high, medium, low)
- [ ] Due dates and reminders
- [ ] Task categories/tags
- [ ] Search functionality
- [ ] Drag-and-drop reordering
- [ ] Export tasks to JSON/CSV
- [ ] Multi-device sync with backend
- [ ] Recurring tasks
- [ ] Subtasks support

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

- GitHub: [@oshan-perera](https://github.com/oshan-perera)

## 🙏 Acknowledgments

- Design inspiration from [Dribbble](https://dribbble.com)
- Icons by [Lucide](https://lucide.dev)
- UI components by [shadcn/ui](https://ui.shadcn.com)
- Color palette inspired by peaceful productivity themes

## ⭐ Show Your Support

Give a ⭐️ if you like this project!

---

<div align="center">

Made with ❤️ and React

</div>

