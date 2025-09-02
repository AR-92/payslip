# payslip

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A web-based payslip management and generation system.

## Description

This application provides a comprehensive solution for managing employee payslips and payroll information. It offers features for creating, viewing, printing, and managing employee salary details with a user-friendly interface.

## Key Features

- Employee payslip generation
- Payroll data management
- Printable payslip templates
- Employee database management
- Responsive web interface
- Offline capability with PouchDB
- Date picker for period selection
- Print-friendly layouts

## Technologies Used

- **HTML5**: Modern markup and semantic elements
- **CSS3**: Styling with Bootstrap framework
- **JavaScript**: Client-side programming language
- **Bootstrap**: Frontend framework for responsive design
- **PouchDB**: Client-side database for offline storage
- **jQuery**: DOM manipulation and event handling
- **Datepicker**: Calendar widget for date selection
- **Print Media**: Print-friendly layouts

## Installation

```bash
# Clone the repository
git clone https://github.com/AR-92/payslip.git
cd payslip

# Run a local server (any static file server will work)
# Python 3
python -m http.server 8000

# Node.js (if you have http-server installed)
npx http-server

# Then open http://localhost:8000 in your browser
```

## Usage

The application includes several key pages:

1. **index.html** - Main dashboard for payslip management
2. **employee.html** - Employee data management
3. **slip.html** - Payslip creation and viewing
4. **print.html** - Print-friendly payslip template

### Key Functionality
- Add and manage employee information
- Generate payslips for specific periods
- View historical payslip data
- Print payslips in a professional format
- Store data locally with offline capability

## Project Structure

```
payslip/
├── index.html                # Main dashboard
├── employee.html             # Employee management
├── slip.html                 # Payslip creation/viewing
├── print.html                # Print-friendly template
├── data.js                   # Data management functions
├── pouchdb.js                # PouchDB library
├── pouchfind.js              # PouchDB find plugin
├── bootstrap-datepicker.js   # Date picker widget
├── bootstrap.min.js          # Bootstrap JavaScript
├── jquery.min.js             # jQuery library
├── popper.min.js             # Popper library
├── perfect-scrollbar.jquery.min.js  # Scrollbar plugin
├── now-ui-dashboard.min.js   # Dashboard JavaScript
├── css/                      # Stylesheets
│   ├── bootstrap.min.css     # Bootstrap CSS
│   └── now-ui-dashboard.css  # Dashboard styling
├── fonts/                    # Web fonts
├── README.md                 # This file
└── LICENSE                   # License information
```

## Data Management

### Employee Information
- Employee ID
- Name and personal details
- Salary information
- Position and department
- Contact information

### Payslip Data
- Pay period (start and end dates)
- Earnings (basic salary, allowances, bonuses)
- Deductions (taxes, insurance, other)
- Net pay calculation
- Payment status

## Offline Capability

The application uses PouchDB for local data storage:
- Data persists between sessions
- Works without internet connection
- Synchronization ready for future server integration
- Indexed data for fast retrieval

## Customization

### Styling
- Bootstrap-based responsive design
- Now UI Dashboard theme
- Custom CSS in the `css/` directory
- Print media queries for payslip printing

### Adding New Features
1. Extend data models in `data.js`
2. Add new UI components as needed
3. Implement additional business logic
4. Update the database schema if required

## Development

### Adding Employees
1. Navigate to the employee management page
2. Fill in employee details in the form
3. Save the information to the local database
4. Verify the employee appears in the list

### Generating Payslips
1. Select an employee from the dashboard
2. Choose the pay period using the date picker
3. Enter earnings and deductions
4. Calculate net pay automatically
5. Save or print the payslip

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature-name`)
6. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

- GitHub: [AR-92](https://github.com/AR-92)