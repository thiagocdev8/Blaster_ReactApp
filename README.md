# Blaster 🐛

A lightweight bug tracking application built with React for managing and organizing bug reports efficiently.

## Features

- **Create Bug Tickets** - Report bugs with title, description, and priority level
- **Priority Levels** - Categorize bugs as Low, Medium, or High priority
- **Edit Tickets** - Update existing bug reports
- **Delete Tickets** - Remove resolved or duplicate bugs
- **Visual Priority Indicators** - Color-coded dots for quick priority identification
- **State Management** - Built with React useReducer for predictable state updates

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone <your-repo-url>
cd blaster
```

2. Install dependencies
```bash
npm install
```

3. Start the development server
```bash
npm start
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## Usage

### Creating a Ticket

1. Fill in the ticket title
2. Add a description of the bug
3. Select a priority level (Low, Medium, or High)
4. Click "Submit"

### Editing a Ticket

1. Click the "Edit" button on any ticket
2. The form will populate with the ticket's current data
3. Make your changes
4. Click "Submit" to save or "Cancel Edit" to discard changes

### Deleting a Ticket

Click the "Delete" button on any ticket to remove it from the list

## Project Structure

```
src/
├── components/
│   ├── TicketForm.js      # Form for creating/editing tickets
│   ├── TicketItem.js      # Individual ticket display
│   └── TicketList.js      # List container for all tickets
├── reducers/
│   └── ticketReducer.js   # State management logic
├── App.js                 # Main application component
├── App.css                # Application styles
└── styles.css             # Additional styling
```

## Technologies Used

- **React** - UI library
- **React Hooks** - useState, useEffect, useReducer for state management
- **CSS** - Custom styling

## State Management

The app uses React's `useReducer` hook for state management with the following actions:

- `ADD_TICKET` - Creates a new ticket
- `UPDATE_TICKET` - Updates an existing ticket
- `DELETE_TICKET` - Removes a ticket
- `SET_EDITING_TICKET` - Sets a ticket for editing
- `CLEAR_EDITING_TICKET` - Clears the editing state

## Known Issues

If experiencing issues with editing tickets not working properly, ensure priority values are consistently typed (numbers vs strings). See the bug fix in the commit history.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Future Enhancements

- [ ] Add ticket status (Open, In Progress, Resolved)
- [ ] Filter tickets by priority
- [ ] Search functionality
- [ ] Persistent storage (localStorage or database)
- [ ] User authentication
- [ ] Ticket assignment to team members
- [ ] Due dates and timestamps
- [ ] Export tickets to CSV/JSON

## Contact

For questions or suggestions, please open an issue in the repository.
