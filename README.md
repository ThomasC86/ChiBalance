# ChiBalance Tongue Analyzer

![Tongue Analyzer](/images/0.png)

## Project Description

ChiBalance Tongue Analyzer is an innovative application designed to assess tongue health through advanced computer vision and data integration. By allowing users to upload images of their tongues, our platform leverages AI algorithms to analyze various attributes such as color, texture, and other features indicative of health conditions. Additionally, users can provide symptom information, enabling the generation of comprehensive health reports. The application seamlessly integrates with hardware components to monitor vital signs, enhancing the depth and accuracy of the analysis.

## Demo Video

[Watch the Demo Video](#)

## Team Members

- Xinran Liu
- Kaijie Lai
- Chloe Yun
- Ho Lok Cheung

## Submission Track

Health & Wellness

## Prizes

We're submitting for the following prizes:

- Best Health Hack
- Most Innovative Use of AI
- Best Integration of Hardware and Software

## Technologies Used

### Frontend

- **React.js**: Building a dynamic and responsive user interface.
  - **Webcam**: Capturing real-time tongue images.
  - **Axios**: Handling HTTP requests for seamless data communication.

### Backend

- **Node.js & Express.js**: Creating a robust and scalable server.
  - **Axios**: Managing API integrations.
  - **Body-Parser & JSON**: Parsing incoming request bodies.
  - **OpenAI**: Utilizing Vision gpt4o for advanced data analysis and predictions.
  - **Python (`predict.py`)**: Handling image classification and predictions.
- **Advanced AI and Computer Vision**
  - **Vision4o Pretrained Model by OpenAI**: Leveraging advanced models for image analysis.
  - **YOLO (You Only Look Once)**: Implementing real-time object detection for enhanced image processing.
  - **Optimized File Transfer**: Utilizing Base64 Encoding and Multipart Form Data for efficient data transmission.

For image analysis, we employed **Vision4o**, a pretrained model by OpenAI, alongside **YOLO** for real-time object detection. These technologies work in tandem to analyze tongue images comprehensively, identifying key health indicators with precision.

### Hardware Backend

- **Flask**: Developing RESTful endpoints for hardware communication.
- **PySerial**: Facilitating serial communication with Arduino.
- **Arduino Integration**: Connecting and managing the MAX30105 heartbeat sensor.
- **Flask Endpoint**: Driven by the Arduino heartbeat sensor to monitor heart rates.

### Cloud & DevOps

- **Defang Cloud**: Orchestrating Docker containers for efficient deployment and scalability.
- **Docker**: Containerizing applications for consistent environments.
- **Shell Scripts**: Automating DevOps processes to streamline development workflows.


### Hardware Components

- **MAX30105 Heartbeat Sensor**: Analyzing heartbeat data to complement tongue health assessments.

## How We Built It

### Frontend Development

We built the frontend using **React.js**, incorporating the **Webcam** API to allow users to capture real-time images of their tongues. **Axios** handles all HTTP requests, ensuring smooth communication between the client and server.

### Hardware Communication

The hardware backend is powered by **Flask**, which communicates with an Arduino device equipped with the **MAX30105 Heartbeat Sensor**. Using **PySerial**, we establish a serial connection between Flask and Arduino, allowing real-time heartbeat monitoring. Flask endpoints driven by Arduino data ensure continuous and reliable data flow.

### Cloud Orchestration

We utilized **Defang Cloud** to orchestrate our Docker containers, ensuring scalable and manageable deployments. Docker containers encapsulate both frontend and backend services, providing consistent environments across development and production.


### Optimized Data Handling

To ensure efficient data transmission, we implemented **Base64 Encoding** and **Multipart Form Data** for file transfers. This optimization reduces latency and enhances the application's responsiveness.

### DevOps Automation

Our DevOps process is streamlined using shell scripts (`run.sh`), automating tasks such as dependency installation, environment setup, and server deployment. This automation accelerates development cycles and minimizes manual intervention.

## Metrics & Algorithms

ChiBalance employs a combination of machine learning algorithms and predefined metrics to assess tongue health. The integration of gpt4o-4 enhances the depth of analysis, providing insightful health recommendations based on both visual and symptom data.

## Learn More

Explore our codebase and contribute to the project on [GitHub](https://github.com/jonlai211/ChiBalance).

## External Resources

- [Defang Cloud](https://defang.io/)
- [Vision4o Pretrained Model](https://openai.com/)
- [YOLO Object Detection](https://pjreddie.com/darknet/yolo/)

## Setup Instructions

### Frontend Setup

```bash
cd client && npm install && npm start
```

### Backend Setup

#### Environment Configuration

Create a `.env` file in the server folder:

```bash
cd server
cp .env.example .env
```

Then add the necessary credentials to the `.env` file.

#### Start the Backend Server

```bash
cd server && npm install && npm run server
```

### Running the Entire Application

Execute the shell script to automate the DevOps process:

```bash
bash ./run.sh
```

## Conclusion

ChiBalance Tongue Analyzer bridges the gap between traditional health assessments and modern technology, providing users with a comprehensive tool for monitoring their tongue health and overall well-being. Through the seamless integration of frontend and backend technologies, advanced AI models, and reliable hardware components, we offer an innovative solution that empowers individuals to take charge of their health.
