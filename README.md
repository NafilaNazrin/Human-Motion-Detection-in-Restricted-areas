# Human-Motion-Detection-in-Restricted-areas
A real-time motion detection system designed to identify and alert for human presence in restricted areas. The system uses OpenCV to analyze live video feeds and triggers email notifications when unauthorized motion is detected.

# Features
Real-Time Detection: Monitors a video feed for human motion, highlighting detected movement in the display.
Email Notifications: Sends an alert email to a designated client when motion is detected.
Cooldown and Warm-Up Phases: Configurable cooldown period between alerts to prevent excessive notifications, and a warm-up period for stabilizing background subtraction.

# Project Overview
This project utilizes OpenCV for motion detection through background subtraction and smtplib for sending email alerts. The background subtraction stabilizes during a warm-up phase before active detection begins, and alerts are limited by a cooldown period.

# Technology Stack
Programming Language: Python
# Libraries:
OpenCV: For video processing and motion detection
smtplib and email.mime.text: For email notifications
NumPy: For array operations and handling image data
# System Requirements
Python 3.7+
Required Python libraries: opencv-python, numpy
# Code Structure
send_email_alert(): Sends an email alert when motion is detected.
motion_detection(): Main function to capture video, process frames for motion, and trigger alerts based on motion detection.
# Configuration
Client Email Setup: In the code, update CLIENT_EMAIL, YOUR_EMAIL, and YOUR_PASSWORD with the respective email addresses and an app-specific password for secure access.



Email Notifications: When human motion is detected, an email alert will be sent to the designated client email.
View Output: A live window will display the camera feed with bounding boxes drawn around detected motion areas.
