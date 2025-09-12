# Employee Management System

A modern, responsive Employee Management System built with React and Vite, featuring role-based authentication and task management capabilities. This application uses localStorage for data persistence and provides separate dashboards for administrators and employees.

## 🚀 Features

### Authentication & Authorization
- **Role-based Access Control**: Separate interfaces for Admin and Employee users
- **Secure Login System**: Email and password authentication
- **Session Management**: Persistent login state using localStorage

### Admin Dashboard
- **Task Creation**: Create and assign tasks to employees
- **Employee Overview**: View all employees and their task statistics
- **Task Management**: Monitor task distribution across the team
- **Real-time Updates**: Live task count updates

### Employee Dashboard
- **Task Overview**: Visual dashboard with task statistics
- **Task Management**: Accept, complete, or mark tasks as failed
- **Task Categories**: Organized by different task types (Design, Development, QA, etc.)
- **Progress Tracking**: Monitor personal task completion rates

### Task Management
- **Task States**: New, Active, Completed, and Failed task states
- **Task Assignment**: Assign tasks to specific employees
- **Task Details**: Title, description, due date, and category
- **Status Updates**: Real-time task status changes

## 🛠️ Tech Stack

- **Frontend**: React 18.2.0
- **Build Tool**: Vite 5.2.0
- **Styling**: Tailwind CSS 3.4.13
- **State Management**: React Context API
- **Data Persistence**: localStorage
- **Development**: ESLint, PostCSS, Autoprefixer

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Employee-Management-System---React---localStorage
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to view the application

## 🚀 Available Scripts

- `npm run dev` - Start the development server
- `npm run build` - Build the project for production
- `npm run preview` - Preview the production build
- `npm run lint` - Run ESLint for code quality checks

## 👥 Default Login Credentials

### Admin Access
- **Email**: `admin@me.com`
- **Password**: `123`

### Employee Access
- **Email**: `e@e.com` (Arjun)
- **Password**: `123`

Additional employee accounts are available with the same password pattern.

## 🏗️ Project Structure

```
src/
├── components/
│   ├── Auth/
│   │   └── Login.jsx              # Login component
│   ├── Dashboard/
│   │   ├── AdminDashboard.jsx     # Admin interface
│   │   └── EmployeeDashboard.jsx  # Employee interface
│   ├── TaskList/
│   │   ├── TaskList.jsx          # Main task list container
│   │   ├── NewTask.jsx           # New task display
│   │   ├── AcceptTask.jsx        # Active task display
│   │   ├── CompleteTask.jsx      # Completed task display
│   │   └── FailedTask.jsx        # Failed task display
│   └── other/
│       ├── Header.jsx            # Navigation header
│       ├── CreateTask.jsx        # Task creation form
│       ├── AllTask.jsx           # Task overview table
│       └── TaskListNumbers.jsx   # Task statistics cards
├── context/
│   └── AuthProvider.jsx          # Authentication context
├── utils/
│   └── localStorage.jsx          # Data persistence utilities
├── App.jsx                       # Main application component
└── main.jsx                      # Application entry point
```

## 🎯 Key Components

### Authentication System
- **Login Component**: Handles user authentication
- **AuthProvider**: Manages authentication state using React Context
- **Role-based Routing**: Redirects users based on their role

### Task Management
- **CreateTask**: Admin interface for creating and assigning tasks
- **TaskList**: Employee interface for viewing and managing tasks
- **Task States**: Handles task lifecycle (New → Active → Completed/Failed)

### Data Management
- **localStorage Integration**: Persistent data storage
- **Context API**: Global state management
- **Real-time Updates**: Live data synchronization

## 🎨 UI/UX Features

- **Responsive Design**: Mobile-friendly interface
- **Dark Theme**: Modern dark color scheme
- **Color-coded Tasks**: Visual task status indicators
- **Interactive Elements**: Hover effects and smooth transitions
- **Clean Layout**: Intuitive user interface

## 🔧 Configuration

The application uses several configuration files:

- `vite.config.js` - Vite build configuration
- `tailwind.config.js` - Tailwind CSS configuration
- `postcss.config.js` - PostCSS configuration
- `package.json` - Project dependencies and scripts

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🐛 Known Issues

- Data persistence relies on localStorage (not suitable for production)
- No server-side validation
- Limited error handling for edge cases

## 🚀 Future Enhancements

- [ ] Backend API integration
- [ ] Database implementation
- [ ] User registration system
- [ ] Email notifications
- [ ] File upload for tasks
- [ ] Advanced reporting features
- [ ] Mobile app development
- [ ] Real-time collaboration

## 📞 Support

For support, email your-email@example.com or create an issue in the repository.

---

**Note**: This is a demo application using localStorage for data persistence. For production use, consider implementing a proper backend with database integration.