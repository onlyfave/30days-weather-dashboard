
# 30days Weather Dashboard

## Overview
The **30days Weather Dashboard** is a Python-based application designed to fetch weather data for multiple cities using the OpenWeather API. It saves the fetched weather data to an AWS S3 bucket for storage, demonstrating best practices in API integration, cloud resource management, and secure credentials handling.

## Features
- Fetches real-time weather data for specified cities.
- Displays temperature, humidity, and weather conditions.
- Saves weather data securely to an AWS S3 bucket.
- Implements error handling for API and cloud service interactions.

## Technologies Used
- **Programming Language:** Python
- **API Service:** OpenWeather API
- **Cloud Service:** AWS S3
- **Libraries:**
  - `boto3` for AWS interactions
  - `requests` for HTTP requests to the OpenWeather API
  - `dotenv` for managing environment variables

## Project Structure
```
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests/
  data/
  .env
  .gitignore
  requirements.txt
```

### File Descriptions
- `src/weather_dashboard.py`: Main script for fetching weather data and interacting with AWS S3.
- `.env`: Stores sensitive credentials such as API keys and AWS bucket names.
- `requirements.txt`: Lists the dependencies required for the project.

## Setup Instructions

### Prerequisites
Ensure the following are installed:
- Python 3.8+
- AWS CLI
- Git

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/onlyfave/30days-weather-dashboard.git
   cd 30days-weather-dashboard
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure environment variables in a `.env` file:
   ```plaintext
   OPENWEATHER_API_KEY=01a1ec452e4adb14c36d7121723ddc04
   AWS_BUCKET_NAME=weather-dashboard
   AWS_DEFAULT_REGION=us-east-1
   ```

4. Configure AWS credentials:
   ```bash
   aws configure
   ```

5. Run the application:
   ```bash
   python3 src/weather_dashboard.py
   ```

## Screenshots

1. **Application Output:**

![Screenshot 2025-01-26 165945](https://github.com/user-attachments/assets/3df8ec33-6476-4bb3-a331-b49d2d76374a)

2. **AWS S3 Bucket Configuration:**

![Screenshot 2025-01-26 173554](https://github.com/user-attachments/assets/2acbcb7f-d9e8-4b6b-a483-5f29019ad7b0)


3. **Error Handling:**
   
![Screenshot 2025-01-26 174257](https://github.com/user-attachments/assets/5e68c1a9-4016-42cc-8942-434bee81d8cb)

4. **AWS S3 Output:**
   
![Screenshot 2025-01-26 173717](https://github.com/user-attachments/assets/8b2fb30e-1754-4b44-8e50-d4e480041167)


## What I Learned
- **AWS S3 Bucket Management:** Creating, managing, and integrating S3 buckets with Python.
- **Secure Credential Handling:** Using environment variables to manage sensitive information securely.
- **API Integration:** Best practices for consuming external APIs in Python.
- **Error Handling:** Managing and logging errors in distributed systems.
- **Git Workflow:** Managing version control for project development.

## Future Enhancements
- Add weather forecasting for upcoming days.
- Implement a graphical user interface (GUI) for better usability.
- Integrate advanced data visualizations using libraries like Matplotlib or Plotly.
- Expand support for more cities and internationalization.
- Automate testing using frameworks like Pytest.
- Set up a CI/CD pipeline for streamlined deployments.

## Acknowledgements
Special thanks to:
- The DevOps and Python communities for their invaluable resources.
- [OpenWeather](https://openweathermap.org/) for providing weather data.
- [AWS](https://aws.amazon.com/) for cloud storage and infrastructure.

## Contact
For any questions or feedback, feel free to reach out:
- **Name:** Onyeneke Favour
- **LinkedIn:** [Onyeneke Favour](https://www.linkedin.com/in/favour-onyeneke-2b2881297/)
- **GitHub:** [onlyfave](https://github.com/onlyfave)

---

Enjoyed this project? Please star the repository on GitHub and share your feedback!

