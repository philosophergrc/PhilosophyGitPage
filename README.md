# Philosophy Topics Interactive Web App
This is an interactive educational web application designed to present various philosophy course topics and modules in an engaging, mobile-friendly way. Users can explore chapters via a sidebar or dropdown menu, view custom module cards with descriptions and links, and enjoy responsive behavior across devices.

## Features

- **Modular Layout**: Organized topics and sub-modules for multiple philosophy courses.
- **Responsive Design**: Optimized layout for mobile and desktop (stacked mobile view, dropdown navigation).
- **Image Hover Effects**: Module images expand on hover for a more interactive experience and to preview the course.
- **Dynamic Content Loading**: Topics and modules are generated dynamically from a structured JavaScript object.
- **Neon Styling**: Custom theme with neon yellow accent colors and hover effects using custom CSS.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- media queries

## Mobile Support

This app is fully responsive. On small screens:
- Sidebar is hidden.
- A dropdown menu allows users to select a topic.
- Modules magically appear beneath the dropdown upon selection.

## Accessibility & Screen Reader Improvements

This application has been carefully enhanced to ensure accessibility and a smooth experience for users relying on screen readers and keyboard navigation. Key improvements include:

- **Explicit ARIA Roles and Attributes**  
  - Each topic button is marked with `role="tab"` to inform assistive technologies that these are part of a tablist interface.  
  - `aria-selected` dynamically indicates which tab is currently active, improving clarity on the user’s location within the navigation.

- **Clear and Descriptive Labels**  
  - Buttons and interactive elements include explicit `aria-label` attributes, providing concise and meaningful descriptions for screen reader users.  
  - Module images have meaningful `alt` text, either derived from the module title or fallback text (“Module image”) to describe visuals contextually.

- **Keyboard Accessibility**  
  - All interactive controls are reachable and operable via keyboard using `tabindex="0"`, ensuring users can navigate without a mouse.  
  - Focus styles and roles improve usability for keyboard users, supporting seamless navigation through topics and modules.

- **Semantic HTML and ARIA**  
  - Semantic roles like `role="tab"` paired with `tabindex` support assistive technologies in understanding the page structure and interaction model.  
  - Module cards are made keyboard-focusable and labeled with `aria-label` for clear identification.

- **Optimized Link Behavior**  
  - Links within modules are keyboard accessible and clearly marked, avoiding redundant tab stops to streamline navigation.

These efforts aim to create an inclusive educational experience that meets accessibility standards and provides equal access to content for all users.

## Project Structure

- index.html – Main application layout and script logic
- /images/ – Folder containing topic-related preview images
- JavaScript – Handles topic selection and module rendering