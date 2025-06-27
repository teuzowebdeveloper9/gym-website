# Gym Website - Svelte Project

## Overview

This project is a responsive gym website built using Svelte. It was developed as a refresher exercise to reinforce and update my Svelte skills after a period of not using the framework. The experience of creating this project was both enjoyable and educational.

## Technical Details

### Svelte Features Utilized

- **Reactive Declarations**: Leveraged Svelte's reactive statements for efficient state management.
- **Stores**: Implemented `writable` stores from Svelte to maintain a responsive modal state across components.
- **Conditional Rendering**: Utilized `#if` blocks for handling responsive design logic.
- **List Rendering**: Employed `#each` blocks for efficiently mapping and rendering arrays of objects in the frontend.

### Additional Technologies

- **Tailwind CSS**: Integrated for rapid UI development and consistent styling.
- **Component Architecture**: Implemented a well-structured component hierarchy for improved maintainability and reusability.

## Project Structure

The project follows a modular component-based architecture, with clear separation of concerns:

- `src/components`: Contains reusable Svelte components
- `src/routes`: Defines the routing structure of the application
- `src/lib`: Houses utility functions and shared resources
- `src/utils`: Stores data objects and helper functions

## Responsive Design

Special attention was given to ensuring the website is fully responsive, adhering to modern frontend development standards. The use of Tailwind CSS and Svelte's conditional rendering facilitated the creation of a fluid, adaptive layout.

## Project Creation

**Note**: The traditional method of creating a Svelte project is now deprecated. The current recommended approach is to use:

npx create-svelte@latest my-app
