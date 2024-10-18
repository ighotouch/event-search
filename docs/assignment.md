# Next.js Assignment

## Overview

This project is a simple Next.js application built with TypeScript, TailwindCSS, and React. Your task is to implement a **search feature** for users and display the search results in a table. Additionally, you will need to provide an option to **clear the search results** and display all users again.

## Tech Stack

- **Framework**: Next.js (React)
- **Language**: TypeScript
- **Styling**: TailwindCSS

## Assignment Tasks

### Primary Objective: User Search Functionality

1. **Search Input**:

   - Add a search input field at the top of the user table.
   - Allow the user to type in the search input to filter users by **name** or **email**.
   - Implement debouncing (optional but recommended) to avoid triggering too many search requests as the user types.

2. **Displaying Search Results**:

   - When the user enters a search query, update the table to display only the users that match the search term (by name or email).
   - If no users match the search term, display a message such as "No users found."

3. **Clear Search**:

   - Add a "Clear Search" button or option near the search input field.
   - When this button is clicked, clear the search input and restore the table to show all users.

4. **State Management**:
   - Store the user data in the component state or context.
   - Update the state based on the search query and clear search actions.

## Additional Tasks for the Assignment

### Detailed User View

- **Objective**: Implement a user-friendly modal or separate page that displays detailed information about a user when their name is clicked in the user table.

### Bonus Objectives:

- **Styling**:

  - Ensure that the search input, table, and clear button are styled using TailwindCSS.
  - The layout should be responsive and look good on different screen sizes.

- **User Experience Enhancements**:

  - Implement **debouncing** for the search input to delay the search until the user stops typing (for example, wait 300ms after the user stops typing before applying the search).
  - Use a **loading indicator** when fetching user data or when the search query is being processed.

- **Performance Considerations**:

  - Optimize the search functionality by using **memoization** or other techniques to avoid unnecessary re-renders.

- **Unit tests**
  - Implement unit tests.

### Data Source

You can use static mock data or fetch the user list from an external API such as [JSONPlaceholder Users](https://jsonplaceholder.typicode.com/users). Make sure the table is populated with users, and the search functionality works on this dataset.

## Project Structure

The project follows a standard Next.js file structure:

```bash
.
├── components      # Reusable React components
├── app             # Next.js pages
├── public          # Public assets (images, fonts, etc.)
├── styles          # Tailwind CSS config and global styles
├── types           # TypeScript interfaces and types
├── utils           # Utility functions (if needed)
├── hooks           # Custom hooks
└── Docs            # How we work at In2event
```

### Explanation:

- **Primary Objective**: The assignment focuses on implementing a search feature for filtering users and providing the ability to clear the search results.
- **Bonus Objectives**: Includes optional tasks such as debouncing the search input, adding a loading indicator, and ensuring responsiveness using TailwindCSS.
- **Review Criteria**: Outlines the key areas you will evaluate during the code review: code quality, completeness, responsiveness, state management, and performance.
