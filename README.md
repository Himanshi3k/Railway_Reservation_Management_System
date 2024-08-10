
# Railway Reservation Management System

## Overview

This project is a simple railway reservation system that allows users to view train details, make reservations, cancel reservations, and check PNR status. The system is divided into two main parts: the admin end and the user end implemented in python using file handling.

## Features

### Admin End

1. **Adding Train Details**: 
   - The admin can enter new train details into the system, including train number, train name, date of journey, departure and arrival destinations, and time.
   - These details are stored in a CSV file named `traindet.csv`, which is used for referencing during user interactions.

2. **Viewing Train Details**:
   - The admin can view all the existing train details stored in the system, helping them manage the available train data.

### User End

1. **Train Details**:
   - Users can view the details of all available trains, including their schedule and route information, as stored in the system.

2. **Reservation**:
   - Users can reserve seats on a selected train for a specific date, provided the train is available on that date and the departure and arrival destinations match the user's request.
   - The system checks the availability of seats (with a maximum of 100 seats per train) and allows users to choose between AC and NON-AC classes.
   - Upon successful reservation, the user is provided with a PNR number, and the details are stored in a CSV file named `passen.csv`.

3. **Cancel Reservation**:
   - Users can cancel their reservation by providing their PNR number. The system then removes the corresponding entry from the `passen.csv` file.

4. **PNR Status**:
   - Users can check the status of their reservation by entering their PNR number, which will display details like train number, departure time, and seat class.

## Files Used

- **`traindet.csv`**: Stores the train details entered by the admin.
- **`passen.csv`**: Stores the reservation details of users, including the PNR number and other relevant information.

