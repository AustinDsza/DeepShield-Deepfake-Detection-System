# Deep Shield

Deep Shield is an AI-powered solution designed to provide comprehensive security and detection against potential threats. This repository includes the codebase, models, and necessary files to deploy and test the system locally or in production environments.

## Features

- **Deepfake Detection**: Detects deepfake images using advanced AI algorithms.
- **Full-Stack Application**: Includes both a Django-based backend and a React Native mobile app.
- **Customizable and Scalable**: Flexible architecture for deployment on various platforms.
- **Real-time Analysis**: Processes data in real-time for immediate threat identification.
- **Seamless Integration**: React Native app interacts with the backend API smoothly.

## Table of Contents

- [Project Structure](#project-structure)
- [Installation](#installation)
- [Backend Setup](#backend-setup)
- [Mobile App Setup](#mobile-app-setup)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Project Structure

```
Deep_Shield/
├── backend/           # Django backend for deepfake detection API
│   ├── all/
       ├── templates/
       ├── detector/
       ├── media/
       ├── views.py
       ├── urls.py       # HTML files for web-based frontend
│   ├── backend/        # Static files (CSS, JS, images)
│   ├── manage.py      # Django management script
│   ├── requirements.txt   # Backend dependencies
├── mobile-app/        # React Native app
│   ├── App.js         # Main entry point for the app
│   ├── package.json   # Dependencies for the mobile app
├── README.md          # Project documentation
└── LICENSE            # License file
```

## Installation

**Note** : This react Native and Frontend app in Django use a API which is created with backend folder using Rest Framework , 
You have to perform port forwarding in vscode and forward 8000 and make url public that public url you have to used in react native and in scripts.js in backend/all/static/scripts.js

### Backend Setup

1. Navigate to the backend folder:
   ```bash
   cd backend
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run database migrations:
   ```bash
   python manage.py migrate
   ```

4. Start the Django server:
   ```bash
   python manage.py runserver
   ```

5. The API will be available at `http://127.0.0.1:8000/`.

### Mobile App Setup

1. Navigate to the mobile-app folder:
   ```bash
   cd mobile-app
   ```

2. Install the required dependencies using npm or yarn:
   ```bash
   npm install
   ```

   or

   ```bash
   yarn install
   ```

3. Start the Expo development server:
   ```bash
   npx expo start
   ```

4. Use the Expo Go app on your mobile device to scan the QR code and run the app.

## Usage

1. Use the backend API to upload an image for deepfake detection.
2. The React Native app interacts with the backend to provide a seamless user experience.
3. Monitor results on the app or through the web interface provided by the backend.

## Dependencies

- **Backend**:
  - Django
  - Pillow (for image handling)
  - TensorFlow/PyTorch (for AI models)
  - Other dependencies in `backend/requirements.txt`

- **Mobile App**:
  - React Native
  - Expo (compulsory)
  - Axios (for API communication)
  - Other dependencies in `mobile-app/package.json`

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Add new feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

