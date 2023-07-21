# Overview

This project consists of two main components:

1. ESP32 Firmware written in C. This firmware controls the connection of the ESP32 microcontroller to WiFi networks and TCP servers.
2. A Xamarin.Mac application written in C#. This application provides a user interface and control for the ESP32 device.

## ESP32 Firmware

The ESP32 firmware is responsible for:

- Managing the WiFi connection: Connecting, reconnecting in case of disconnection, and handling failure after multiple retries.
- Handling IP events: The firmware responds to events such as the successful acquisition of an IP address.
- Connecting to a TCP server: This includes handling the connection process, reading from the server, and responding to specific server messages.

The firmware is written in C and designed to be run on an ESP32 microcontroller.

## Xamarin.Mac Application

The Xamarin.Mac application is an interface for the ESP32 device. It provides control for the device and presents the device's status to the user.

The application is written in C# and designed to be run on macOS. It is composed of:

- AppDelegate.cs: This file provides application-level behavior and lifecycle management. This is where you would handle global application events.
- ViewController.cs: This file provides the control logic for your main view (or window). This is where you would put the logic to handle user interactions.
- Main.cs: This file provides the application's entry point.

This project was developed under Professor Rongwei Mao at The University of California, Irvine.
