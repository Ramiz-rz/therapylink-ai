# TherapyLink | AI-Assisted Mental Wellness Application

TherapyLink is my Final Year Project, built as an AI-assisted mental wellness application that combines conversational AI, sentiment analysis, facial emotion recognition, mood tracking, psychological assessments, and access to professional resources in one mobile application.

The goal was to explore how AI can be integrated into a practical mobile application to provide personalized mental wellness support while keeping the system focused on responsible and educational use.

> **Disclaimer:** TherapyLink is an academic and research project. It is not a replacement for a licensed psychologist, psychiatrist, doctor, or other healthcare professional.

---

## Overview

Mental wellness applications often provide isolated features such as mood tracking, chat support, or assessments. TherapyLink brings several of these capabilities together into a single application.

The application allows users to:

* Interact with an AI-based conversational assistant
* Communicate through text and voice
* Receive AI-generated conversational responses
* Analyze sentiment from user input
* Detect facial emotions through the camera
* Track changes in mood
* View mood trends and 24-hour mood graphs
* Complete psychological assessments
* Receive personalized stress-relief suggestions
* Find nearby mental health clinics and professionals
* Securely authenticate through Firebase

The project combines mobile development, machine learning, natural language processing, computer vision, cloud services, and backend technologies.

---

## Key Features

### AI Conversational Assistant

Users can communicate with TherapyLink through natural language.

The conversational system uses GPT-based responses to provide supportive and context-aware interactions.

**Flow:**

```text
User Input
    ↓
Text / Voice Processing
    ↓
AI Conversation
    ↓
Response Generation
    ↓
Text Response
    ↓
Voice Output
```

---

### Voice Interaction

TherapyLink supports voice-based interaction so users can communicate without typing.

The system processes spoken input and converts the generated response back into speech.

This makes the interaction more natural and accessible.

---

### Sentiment Analysis

User messages can be analyzed to identify the overall emotional tone of the conversation.

The system uses NLP techniques and transformer-based models to process text and identify sentiment patterns.

```text
User Message
      ↓
Text Processing
      ↓
NLP Model
      ↓
Sentiment Analysis
      ↓
Mood / Emotion Data
```

---

### Facial Emotion Detection

TherapyLink also explores computer vision for emotion recognition.

The camera can be used to analyze facial expressions and identify emotional states.

The project uses machine learning and computer vision technologies to process facial information and extract emotion-related signals.

---

### Mood Tracking

TherapyLink stores mood-related information and presents it through visual graphs.

Users can monitor how their mood changes over time.

The application includes:

* Mood history
* Daily mood tracking
* 24-hour mood graphs
* Visual trend analysis

This provides users with a simple way to observe patterns in their emotional state.

---

### Psychological Assessments

The application includes psychological assessment functionality designed for educational and awareness purposes.

Assessment results can help users understand their responses and identify areas that may require additional attention.

The results are not intended to provide a medical diagnosis.

---

### Personalized Stress-Relief Suggestions

Based on user interactions and mood-related information, TherapyLink can provide personalized suggestions such as:

* Breathing exercises
* Relaxation techniques
* Stress-management activities
* General wellness recommendations

---

### Mental Health Resource Locator

TherapyLink integrates Google Maps to help users locate nearby clinics and professional resources.

```text
User Location
      ↓
Google Maps API
      ↓
Nearby Mental Health Resources
      ↓
Map / Location Results
```

This provides a bridge between AI-assisted support and professional resources.

---

### Firebase Authentication

Firebase is used for secure user authentication and application services.

The system supports authenticated user access while keeping sensitive application data protected.

---

## System Architecture

The overall TherapyLink workflow can be summarized as:

```text
                    ┌──────────────────┐
                    │      User        │
                    └────────┬─────────┘
                             │
                    Text / Voice / Camera
                             │
                             ▼
                 ┌────────────────────────┐
                 │   Flutter Application  │
                 └────────────┬───────────┘
                              │
            ┌─────────────────┼─────────────────┐
            │                 │                 │
            ▼                 ▼                 ▼
       NLP / AI          Computer Vision    Voice Processing
            │                 │                 │
            ▼                 ▼                 ▼
      Sentiment          Facial Emotion      Speech
       Analysis            Detection        Processing
            │                 │                 │
            └─────────────────┼─────────────────┘
                              │
                              ▼
                    ┌──────────────────┐
                    │ Analysis Layer   │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │ Personalized     │
                    │ Support          │
                    └────────┬─────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
              ▼              ▼              ▼
          AI Response    Mood Tracking   Resources
              │              │              │
              ▼              ▼              ▼
          User Support    Graphs       Google Maps
```

---

## Technology Stack

### Mobile Application

* Flutter
* Dart

### Artificial Intelligence

* Python
* TensorFlow
* PyTorch
* Hugging Face
* BERT
* GPT-4

### Natural Language Processing

* Sentiment Analysis
* Transformer Models
* BERT
* Text Processing
* Conversational AI

### Computer Vision

* Facial Emotion Recognition
* Image Processing
* Deep Learning

### Backend

* Node.js
* Python

### Database and Cloud

* Firebase
* Firebase Authentication
* Firebase services

### APIs

* Google Maps API
* AI APIs
* Speech / Voice services

### Data Visualization

* Matplotlib
* Plotly

### Development Tools

* Git
* GitHub
* VS Code
* Android Studio

---

## Project Structure

The project follows a Flutter-based application structure with additional backend and AI components.

```text
fyp_therapylink/
│
├── android/
├── ios/
├── linux/
├── macos/
├── windows/
├── web/
│
├── assets/
│
├── lib/
│   ├── screens/
│   ├── widgets/
│   ├── services/
│   ├── models/
│   └── ...
│
├── functions/
│
├── dataconnect/
├── dataconnect-generated/
│
├── test/
│
├── firebase.json
├── firestore.rules
├── firestore.indexes.json
├── pubspec.yaml
├── pubspec.lock
└── README.md
```

---

## Core Workflow

The main application workflow follows this structure:

```text
User Interaction
       ↓
Text / Voice / Facial Input
       ↓
Data Processing
       ↓
AI / ML Analysis
       ↓
Emotion & Sentiment Understanding
       ↓
Response Generation
       ↓
Personalized Support
       ↓
Mood Tracking
       ↓
Professional Resources
```

---

## AI and Machine Learning Components

One of the main objectives of this project was to understand how multiple AI techniques can work together inside a real application.

### NLP

Natural language processing is used to process user messages and extract meaningful information from text.

Technologies explored include:

* BERT
* Hugging Face Transformers
* Sentiment analysis
* Text classification
* GPT-based conversational responses

### Computer Vision

Computer vision is used for facial emotion recognition.

The system processes facial expressions and attempts to identify emotional states from visual input.

### Conversational AI

GPT-based models are integrated to generate natural-language responses.

The conversational component allows users to interact with the application in a more natural way compared with traditional rule-based applications.

---

## Security and Privacy

Because TherapyLink works with sensitive user interactions, security was considered throughout the application.

The project includes:

* Firebase authentication
* Authenticated user access
* Secure handling of application data
* Protection of sensitive configuration files
* Separation of credentials from source code

### Important

API keys, Firebase credentials, service-account files, and other secrets should **never** be committed to GitHub.

For example:

```text
assets/google_speech.json
```

is intentionally excluded from the public repository.

Developers should configure their own credentials locally when running services that require authentication.

---

## Running the Project

### Requirements

Before running TherapyLink, install:

* Flutter SDK
* Dart SDK
* Android Studio
* VS Code
* Git

Verify Flutter:

```powershell
flutter doctor
```

---

### Clone the Repository

```powershell
git clone https://github.com/Ramiz-rz/therapylink-ai.git
cd therapylink-ai
```

---

### Install Dependencies

```powershell
flutter pub get
```

---

### Run the Application

Connect an Android device or start an Android emulator.

Then:

```powershell
flutter run
```

You can also check available devices:

```powershell
flutter devices
```

---

## Firebase Configuration

TherapyLink uses Firebase services.

To run the project with your own Firebase environment, configure Firebase for your application rather than using private credentials from the original development environment.

Depending on your setup, you may need to configure:

* Firebase Authentication
* Firestore
* Firebase project configuration
* Android Firebase configuration
* iOS Firebase configuration

Do not commit private service-account credentials or API keys.

---

## Google Maps Configuration

The application uses Google Maps functionality for locating relevant professional resources.

To use Google Maps with your own project:

1. Create a Google Cloud project.
2. Enable the required Maps APIs.
3. Create an API key.
4. Configure the key for your target platform.
5. Add the configuration locally.

Do not commit private API credentials to GitHub.

---

## Screenshots

Screenshots of the application can be added here to show the main functionality.

Recommended structure:

```text
screenshots/
├── home.png
├── ai-chat.png
├── voice-chat.png
├── mood-tracking.png
├── emotion-detection.png
├── assessment.png
└── maps.png
```

Example:

```markdown
## Screenshots

### AI Conversation

![AI Conversation](screenshots/ai-chat.png)

### Mood Tracking

![Mood Tracking](screenshots/mood-tracking.png)

### Emotion Detection

![Emotion Detection](screenshots/emotion-detection.png)

### Mental Health Resources

![Mental Health Resources](screenshots/maps.png)
```

---

## What I Learned

Building TherapyLink gave me practical experience in combining multiple technologies into one application rather than working on isolated machine learning experiments.

Some of the main areas I worked with include:

* Building a Flutter application
* Integrating AI APIs into a mobile application
* Working with NLP and transformer models
* Implementing sentiment analysis
* Exploring facial emotion recognition
* Working with speech and voice interaction
* Integrating Firebase
* Working with Google Maps APIs
* Connecting frontend applications with backend services
* Managing application data
* Visualizing mood-related information
* Handling API credentials and application security
* Structuring a larger final-year software project

The project also helped me understand the challenges involved in moving an AI model from experimentation into an actual user-facing application.

---

## Limitations

TherapyLink is an academic project and has several limitations.

* AI-generated responses may not always be accurate.
* Emotion detection is not guaranteed to correctly represent a user's actual emotional state.
* Sentiment analysis can be affected by language and context.
* The application should not be used for medical diagnosis.
* AI responses should not replace professional mental health care.
* Production deployment would require additional security, testing, monitoring, and clinical validation.

---

## Future Improvements

Potential improvements include:

* More advanced emotion recognition models
* Better multilingual NLP support
* Improved conversational memory
* More accurate personalization
* Real-time AI monitoring and analytics
* Improved voice interaction
* Better accessibility
* More comprehensive mental wellness resources
* Stronger privacy and security controls
* Cloud-based production deployment
* Model evaluation using larger and more diverse datasets

---

## Academic Project

**Project:** TherapyLink - AI-Assisted Mental Wellness Application

**Type:** Final Year Project

**Degree:** BS Information Technology

The project was developed as part of my undergraduate studies and combines mobile development, artificial intelligence, machine learning, NLP, computer vision, and cloud technologies.

---

## Project Team

TherapyLink was developed as a Final Year Project by:

* Muhammad Rameez
* Azam Ali
* Muhammad Ahmad Bhatti
* Muhammad Zeeshan Ali
---

## Author

### Muhammad Rameez

AI/ML Engineer focused on building practical AI applications, RAG pipelines, NLP systems, automation workflows, and full-stack products.

**GitHub:** https://github.com/Ramiz-rz

**LinkedIn:** https://linkedin.com/in/rameez-aslam/

---

## Disclaimer

TherapyLink is an academic AI-assisted mental wellness project created for educational and research purposes.

The application does not provide medical diagnosis or professional psychological treatment. Users experiencing serious mental health concerns should seek help from a qualified healthcare professional.

---

## License

This project was developed as an academic Final Year Project.

Please contact the author before reusing substantial portions of the source code, models, assets, or project materials for commercial purposes.
