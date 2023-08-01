# Battery Percentage Notifier

This is a Python script that periodically checks the battery percentage of your device and displays a notification with the current battery level. The script uses the `psutil` library to get the battery information and the `plyer` library to display the notification.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Configuration](#configuration)
4. [Acknowledgments](#acknowledgments)
5. [Documentation](#documentation)

## Installation

1. Ensure you have Python installed on your system. You can download Python from the official website: [Python.org](https://www.python.org/downloads/)

2. Install the required dependencies using pip:

```
pip install psutil plyer
```

## Usage

1. Run the Python script in a Python environment with the required dependencies installed.

2. The script will run in the background and periodically check the battery percentage of your device.

3. When the battery percentage is checked, a notification will be displayed with the current battery level.

## Configuration

There are no specific configuration options for this script. However, you can modify the time interval for checking the battery percentage by changing the `time.sleep()` value. The current value of `60 * 60` means the script will check the battery percentage every 60 minutes.

You can adjust this value to your preferred interval. For example, if you want to check the battery percentage every 30 minutes, you can change it to `30 * 60`.

## Acknowledgments

The Battery Percentage Notifier was created by Harsh Gupta (Desparete Enuf) as a simple utility to notify users about their device's battery level. The code is provided here for reference and learning purposes.

## Documentation

The script uses the following libraries and concepts:

1. **psutil**: The `psutil` library is used to get the battery information of the device. The `sensors_battery()` function returns a `Battery` object that contains battery-related information, such as the current battery percentage.

2. **plyer**: The `plyer` library is used to display notifications on the system. The `notification.notify()` function is used to show the battery percentage as a notification. The `title` parameter specifies the title of the notification, and the `message` parameter contains the battery percentage information.

3. **Time Sleep**: The `time.sleep()` function is used to add a delay between each battery check. The current value of `60 * 60` means the script will check the battery percentage every 60 minutes. This interval can be adjusted as per the user's preference.

4. **Infinite Loop**: The script runs in an infinite loop (`while True`) to continuously monitor the battery percentage.

## License

This project is open-source and licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code, but please provide proper attribution to the original creator, Harsh Gupta (Desparete Enuf).
