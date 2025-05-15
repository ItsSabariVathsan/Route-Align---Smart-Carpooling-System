# Route Align - Smart Carpooling System

---
## Table of Contents

- [Project Overview](#project-overview)  
- [Features](#features)  
- [System Architecture](#system-architecture)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Screenshots](#screenshots)  
- [Diagrams](#diagrams)  
- [Technologies Used](#technologies-used)  
- [Contributing](#contributing)    

---
## Project Overview

Route Align is an intelligent carpooling platform designed to optimize urban commuting by leveraging AI-driven route optimization, real-time ride matching, and predictive analytics. This system addresses common limitations of traditional ride-sharing apps by adapting dynamically to real-time traffic conditions and user preferences, thereby reducing traffic congestion, lowering carbon emissions, and improving commuter convenience.

---
## Features

- AI-based ride matching considering route overlap and preferences  
- Real-time dynamic route optimization with live traffic data  
- Predictive analytics to forecast ride demand and improve availability  
- User registration, ride scheduling, and fare estimation  
- Multi-modal transport integration (future scope)  
- User reputation and eco-points system for incentivizing green behavior  

---
## System Architecture

### Ride Matching Module

The Ride Matching Module is the core intelligence engine that identifies optimal pairings between drivers and riders. It uses machine learning algorithms to analyze user preferences, real-time GPS locations, time windows, and route overlap to suggest the best matches. Unlike traditional systems that only match based on destination, this module considers:

- Midpoint overlaps
- Historical trip patterns
- Detour tolerance
- Time flexibility

This ensures high-quality, efficient pairings that minimize travel time and improve user satisfaction.

---
### Dynamic Routing Engine

This module dynamically plans and updates travel routes based on current traffic conditions, weather data, and user locations. It continuously monitors:

- Live traffic feeds (via integrated APIs)
- Road closures or diversions
- Real-time rider/driver positions

By recalculating the fastest and most efficient route for each ride, it ensures that all participants take the shortest and most convenient path, minimizing delays and fuel consumption.

---
### User Management System

The User Management System handles registration, authentication, profile management, and role-based access (Driver or Rider). It supports:

- Secure sign-up and login with validation
- Profile preferences (e.g., preferred travel times, seat availability)
- Rating and reputation tracking
- Eco-point tracking for sustainable travel incentives

This module forms the user interface backbone, ensuring all interactions are personalized and secure.

---

### Database & API Integrations

This foundational layer manages data storage, retrieval, and synchronization. It connects all modules and ensures consistency across the system. Components include:

- **Database**: Stores user profiles, ride history, schedules, and feedback.
- **External APIs**:
    - Traffic and mapping (e.g., Google Maps API)
    - Weather forecasting
    - Location services

The API layer facilitates real-time data flow between internal services and external systems, enabling responsive and context-aware functionalities.

---
## Installation

### Prerequisites
- Python 3.x  
- Virtual environment tool (`venv` or `virtualenv`)  
- Git  
### Setup Instructions

```
bash

# Clone the repository
git clone https://github.com/yourusername/route-align.git
cd route-align

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the application
python app.py 
```

---
## Usage

- Register as a user (driver or rider)
- Offer or request rides via the dashboard
- View optimized routes and live ride status
- Track your eco-points and reputation score

---
## Screenshots
![Create Account](https://github.com/user-attachments/assets/28dbc803-396b-4a3d-845c-37f8a4e7f3da)
![Login Page](https://github.com/user-attachments/assets/c4eb1f6c-4a4a-43ae-a1cd-56493b18b901)
![Dashboard](https://github.com/user-attachments/assets/bfd672a0-353e-483c-8826-8454e93d61de)
![Offer a Ride](https://github.com/user-attachments/assets/6e3311b9-fb33-45f6-9265-42bc4914d8a5)
![Available Rides](https://github.com/user-attachments/assets/a9939609-29cd-458b-b723-7e4650c455cd)
![Request a Ride](https://github.com/user-attachments/assets/58871cff-7024-46f6-b22b-6b48597367e7)
![Ride Requests](https://github.com/user-attachments/assets/64bd2ad0-01ff-49fe-a78e-7f93cb9e09d3)

System architecture diagram

![Full Arch Diagram](https://github.com/user-attachments/assets/00d9aca3-f428-4261-b6a1-ff341ceed371)

---
## Technologies Used

- Python (Flask)
- HTML, CSS, JavaScript
- SQLite
- Machine Learning libraries (e.g., scikit-learn)
- APIs for real-time traffic and mapping

---
## Contributing

Contributions are welcome! Please follow these steps to contribute
1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---
