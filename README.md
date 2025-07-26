IoT Project
Air pollution Monitoring
Report contains complete report with diagrams and codes and results

This project is a real-time, low-cost air quality monitoring system developed using the MQ-135 gas sensor, NodeMCU ESP8266, and Arduino Uno. It detects air pollutants and displays the readings in PPM on a 16x2 LCD screen. The system also includes green and red LEDs, a buzzer, and a potentiometer for LCD contrast control. Based on the PPM levels, it triggers visual and audio alerts to indicate whether the air quality is Normal, Medium, or Dangerous.

The system connects to the internet using the ESP8266 Wi-Fi module and sends real-time sensor data to the ThingSpeak cloud platform using HTTP POST requests secured via a unique API key. This enables continuous remote monitoring, data logging, and visualization through ThingSpeak dashboards. The project ensures secure communication using WPA/WPA2 Wi-Fi encryption, along with proper API key authentication to protect the data channel.

In addition to monitoring, the system includes a predictive module. The air quality data stored in ThingSpeak is exported and preprocessed using Python, where time-based features such as hour, day, and month are extracted. A Decision Tree Classifier is trained to predict air quality categories: Good, Moderate, Unhealthy, and Very Unhealthy. The model achieves an accuracy of 91%, an F1-score of 0.87, and a mean squared error of 0.09, making it effective for forecasting pollution trends.

It combines sensor-based real-time alerting, cloud IoT integration, and machine learning-based forecasting, providing both immediate awareness and future insights into air quality conditions.
