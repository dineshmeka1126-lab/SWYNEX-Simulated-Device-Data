import csv
import random
import time
from datetime import datetime

FILE_NAME = "device_data.csv"

with open(FILE_NAME, "w", newline="") as file:
    writer = csv.writer(file)

    writer.writerow([
        "Timestamp",
        "Temperature_C",
        "Humidity_Percent",
        "Light_Lux"
    ])

    for i in range(20):
        timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")

        temperature = round(random.uniform(20, 35), 2)
        humidity = round(random.uniform(40, 80), 2)
        light = round(random.uniform(100, 1000SWYNEX-Simulated-Device-Data
│
├── simulated_device_data.py
├── device_data.csv
└── README.md# SWYNEX Simulated Device Data

## Project Description

This project generates simulated IoT sensor readings using Python and stores the data in a CSV file.

## Sensors Simulated

* Temperature
* Humidity
* Light intensity

## Technologies Used

* Python
* CSV
* Random
* DateTime

## Features

* Generates timestamped sensor readings
* Simulates temperature, humidity and light values
* Stores readings in `device_data.csv`
* Displays readings in the terminal

## How to Run

Run the following command:

```bash
python simulated_device_data.py
```

The generated sensor readings are automatically stored in `device_data.csv`.

## Task

This project was completed as part of Task 2 of the SWYNEX internship.
), 2)

        writer.writerow([
            timestamp,
            temperature,
            humidity,
            light
        ])

        print(
            f"{timestamp} | "
            f"Temperature: {temperature}°C | "
            f"Humidity: {humidity}% | "
            f"Light: {light} lux"
        )

        time.sleep(1)

print("\nSimulated device data saved successfully to", FILE_NAME)# SWYNEX-Simulated-Device-Data
A Python-based IoT project that generates timestamped simulated sensor data, including temperature, humidity, and light intensity, and stores the readings in a CSV file for further analysis.
