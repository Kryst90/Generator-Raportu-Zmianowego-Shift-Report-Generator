# Shift Report Generator

A modern web-based tool for creating and sending shift reports.  
Built with pure HTML, CSS, and JavaScript — no backend server required.  
Designed for production teams who need a fast and consistent way to log and share daily activities.

## Features
- **Date, shift, and employee selection** – easy input for structured reporting  
- **Task grid** – add up to 10 activities per report  
- **Automatic time sum** – calculates total hours in real-time  
- **Email generation** – creates a ready-to-send email with all activities  
- **Database saving (MS Access)** – automatically stores data in a local `.mdb` file for archiving  

## How It Works
1. Open the `index.html` file in Internet Explorer (required for ActiveX database connection).  
2. Select report date, shift number, and employee name.  
3. Fill in tasks, actions, comments, and time (in minutes).  
4. Click **"Generuj email"** – a new email window will open with all details prefilled.  
5. Data will also be saved into the Access database specified in the script (`raporty.mdb`).  

## Tech Stack
- **HTML5** + **CSS3** – clean and responsive design
- **Vanilla JavaScript** – no external libraries required
- **MS Access (.mdb)** – as local database
- **ActiveXObject** – for direct database operations (Windows only)

## Example UI
![Example Screenshot](docs/example-ui.png) <!-- możesz dodać screenshot do repozytorium -->

## Requirements
- Windows environment
- Internet Explorer (or Edge in IE mode) for ActiveX to work
- MS Access `.mdb` file available on a network/shared drive

## Notes
- You may customize `dbPath` inside the script to point to your company’s Access database location.
- For environments without IE support, consider migrating to a backend API for database write operations.

## License
MIT License – free to use and adapt.
