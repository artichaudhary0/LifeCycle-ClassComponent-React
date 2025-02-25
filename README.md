# React Lifecycle Methods Demo

## 📌 Overview
This project provides an interactive demonstration of React class component lifecycle methods. It allows users to visualize when and how lifecycle methods are called during mounting, updating, and unmounting phases.

## 🚀 Features
- Interactive UI to mount and unmount components
- Displays logs of lifecycle methods execution
- Simulates API calls using `componentDidMount`
- Implements controlled state updates for demonstration
- Highlights both class-based and functional component lifecycles
- Tracks timestamps of lifecycle method executions
- Provides real-time insights into React component behavior
- Offers a counter for triggering state updates

---

## 📂 Project Structure
```
/react-lifecycle-demo
├── src
│   ├── components
│   │   ├── LifecycleDemo.js
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   ├── index.css
├── public
├── package.json
└── README.md
```

---

## 📥 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/artichaudhary0/react-lifecycle-demo.git
   ```

2. Navigate into the project directory:
   ```bash
   cd react-lifecycle-demo
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

---

## 🚀 Usage
To start the application, run:
   ```bash
   npm start
   ```
This will launch the app at `http://localhost:3000/`.

### How It Works
- Click **Mount Component** to load the `LifecycleDemo` component.
- Lifecycle methods execute and log details in the UI.
- Click **Unmount Component** to remove the component, triggering `componentWillUnmount`.
- Click **Trigger Update Phase** to update state, logging the update cycle methods.
- API simulation fetches data asynchronously and updates the component.
- Logs dynamically display timestamps of method executions.

---

## 🔁 React Lifecycle Methods
This project covers all three phases of React component lifecycle:

### **1️⃣ Mounting Phase**
- `constructor()` → Initializes state and binds methods.
- `static getDerivedStateFromProps()` → Syncs state with props before render.
- `render()` → Returns JSX to be displayed.
- `componentDidMount()` → Executes after component mounts, used for API calls.

### **2️⃣ Updating Phase**
- `static getDerivedStateFromProps()` → Called again when props change.
- `shouldComponentUpdate()` → Determines if component should re-render.
- `render()` → Updates the UI based on state/props changes.
- `getSnapshotBeforeUpdate()` → Captures values before update.
- `componentDidUpdate()` → Executes after update, useful for side effects.

### **3️⃣ Unmounting Phase**
- `componentWillUnmount()` → Cleans up before component removal (e.g., removing event listeners, cancelling API calls).

---

## 📊 Future Enhancements
- Add functional component equivalent using `useEffect` hook
- Implement animations for better visualization of updates
- Introduce a dark mode option for improved UI experience
- Allow users to simulate API failures for error handling tests
- Create a settings panel to enable/disable specific lifecycle logs
- Develop an analytics dashboard for tracking lifecycle execution patterns

---

## 👤 Author
Arti Chaudhary
