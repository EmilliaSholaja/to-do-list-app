React To-Do List App
This is a simple To-Do List application built with React, demonstrating fundamental React concepts. The project strictly uses useState for state management and props for data passing between components.
The app uses Font Awesome for all icons and the uuid library to ensure each new to-do item has a unique, stable identifier.
Features

- Add new to-do items to the list.
- Delete to-do items from the list.
- Mark to-do items as complete or incomplete by clicking on them.
- Edit to-do items from the list
  Technologies Used
- React: For building the user interface.
- useState Hook: The sole method for managing the application's state.
- Props: For passing data and callback functions from parent components to their children.
- Font Awesome: For scalable vector icons (e.g., a checkmark and a trash icon).
- uuid: A library used to generate unique IDs for each to-do item, which is crucial for React's list rendering performance.
- JavaScript, HTML5, CSS3: The foundational web technologies.
  How It Works
- State Management: The main list of to-do items is stored in the top-level component's state using useState. This centralizes the data and ensures all changes are handled from a single source of truth.
- Component Communication: Functions (such as addTodo, deleteTodo, and toggleComplete) are defined in the parent component and passed down as props to the child components. When an action is triggered (e.g., a button click in a child component), it calls the prop function, which updates the state in the parent, causing the UI to re-render with the new data.
- Unique Keys: Every time a new to-do item is added, the uuid library generates a unique ID for it. This ID is used as the key prop when rendering the list of items, preventing bugs and optimizing performance.
  Prerequisites
- Node.js
- npm
  How to Run the Project
- Clone the repository:
  git clone https://github.com/your-username/your-repository.git
  cd your-repository

- Install dependencies:
  npm install

- Start the development server:
  npm start

  The application will open in your default web browser at http://localhost:3000.
  Author

- Sholaja Emillia
  License
  This project is open-source and available under the MIT License.
