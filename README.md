# Meowmodoro Timer Project

## Overview
The Meowmodoro Timer is a unique, cat-themed productivity timer based on the Pomodoro Technique. This project, designed for Arduino platforms, not only offers a customizable focus and rest period system but also features engaging, cat-inspired interactive elements for a delightful user experience.

## Features
- **Focus and Rest Periods**: A 25-minute focus timer followed by a 5-minute rest timer.
- **Start Message**: Displays "Start / Meowmodoro" message at the beginning of each focus period.
- **Rest Message**: Shows "Rest Time!" on the screen during the rest periods.
- **Touch Sensor Controls**: Utilizes touch sensors for controlling the timer modes.
- **Lifelike Petting Interaction**: Touch sensors mimic the act of petting a cat, enhancing user interaction and adding a playful element to the timer.

## Lifelike Petting Interaction
Our design features lifelike petting interactions, with touch points that precisely mimic those of a real cat. The touch sensors are strategically placed to respond to user interaction, simulating the experience of petting a cat. This feature not only makes the timer more engaging but also adds a soothing and playful aspect to your focus sessions.

## Hardware Requirements
- ESP32
- OLED Display
- Touch Sensors x4

## Software Requirements
- Arduino IDE
- Libraries: U8g2lib, WiFi, ESP8266HTTPClient, ArduinoJson

## Setup and Installation
1. **Hardware Setup**: Connect the OLED display and touch sensors to the Arduino board as per the circuit diagram provided.
2. **Library Installation**: Ensure all required libraries are installed in the Arduino IDE.
3. **Code Upload**: Open the code file with the Arduino IDE, configure your board and port settings, and upload the code to your Arduino board.

## WiFi and OpenAI API Setup
For full functionality of the Meowmodoro Timer, users must set up WiFi and configure the OpenAI (ChatGPT) API. Follow these steps:
1. **WiFi Configuration**: Ensure that the device is connected to a WiFi network. Provide the necessary SSID and password in the code to enable a stable connection.
2. **OpenAI API Setup**: Obtain an API key from OpenAI. This key is essential for accessing the ChatGPT services. Safely store the API key and include it in the code as required.
3. **Code Modification**: Update the `ssid`, `password`, and `apiKey` variables in your code with your WiFi details and OpenAI API key.
4. **Privacy Note**: Never share your API keys or WiFi credentials in public repositories. Always use environment variables or secure methods to handle such sensitive information.

## Usage
Touch the designated sensor to start the timer. The timer begins with the focus period (25 minutes). After the focus period, the timer will automatically switch to a 5-minute rest period, displaying "Rest Time!". The cycle repeats, alternating between focus and rest periods.

## Customization
Modify `focusDuration` and `restDuration` variables in the code to adjust the lengths of the focus and rest periods. Adjust the `displayStartMessage()` and `displayRestMessage()` functions for custom start and rest messages.

## Troubleshooting
- **Connectivity Issues**: If using WiFi, ensure proper credentials and connection settings.
- **Display Problems**: Verify connections and drivers for the OLED display.
- **Sensor Responsiveness**: Check wiring and code setup for the touch sensors.

## Contact
For any issues, questions, or feedback regarding the Meowmodoro Timer project, please feel free to contact us at [myraliym@gmail.com](mailto:myraliym@gmail.com).

## Contributing
Contributions to the Meowmodoro project are welcome. Please send pull requests or issue reports via email or GitHub. 

## License
This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).
