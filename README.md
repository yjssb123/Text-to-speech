Azure-Powered Text-to-Speech with Photorealistic Avatars
This project serves as an advanced demonstration of Microsoft Azure's cutting-edge Text-to-Speech (TTS) capabilities, specifically showcasing the generation of photorealistic talking avatars. The application, built with Streamlit, provides a user-friendly interface to interact with the powerful Azure AI backend, allowing users to submit text and receive a high-quality video of a talking avatar with synchronized lip movements.


  https://github.com/Sgvkamalakar/Azure-Talking-Avatar/assets/103712713/09fc79f9-cc68-4354-bae7-e75e24add235" width="400" height="400"/>

Core Functionality and Technology
The application leverages Azure's batch synthesis API to convert plain text into a lifelike avatar video. The underlying process is as follows:

Input: A user provides text input through the Streamlit interface and selects a desired language and corresponding avatar style.

Batch Synthesis Job: Upon submission, the application sends a request to the Azure Speech Service. This initiates a batch synthesis job, which is designed for offline processing of larger text inputs.

AI-Powered Generation: Azure's AI services then synthesize the audio using a high-quality neural voice and simultaneously generate a photorealistic video of an avatar. The service ensures that the avatar's lip movements are precisely synchronized with the generated speech.

Real-Time Monitoring & Retrieval: The application continuously polls the Azure service to monitor the job status in real-time. Once the synthesis job is successfully completed, the final video is retrieved and displayed directly in the user's browser.

Key Features
Intuitive User Interface: A clean and simple interface built with Streamlit allows users to easily select options, input text, and generate avatars without needing to write any code.

Diverse Language and Avatar Support: The application supports a wide range of languages, each paired with a unique, high-fidelity neural voice and avatar style.

Asynchronous Processing: By using Azure's batch synthesis API, the application can handle longer text inputs efficiently without blocking the user interface.

Real-Time Job Status: Users can track the progress of their synthesis request, from submission to completion.

Supported Languages and Voices
The application supports a variety of languages, each associated with a specific neural voice provided by Azure.

                                                                         
Language	Neural Voice Name
Arabic	ZariyahNeural
Bahasa Indonesian	GadisNeural
Bengali	TanishaaNeural
Chinese Mandarin	XiaoxiaoNeural
Dutch	FennaNeural
English	AvaNeural
French	DeniseNeural
German	KatjaNeural
Hindi	SwaraNeural
Italian	ElsaNeural
Japanese	NanamiNeural
Korean	SunHiNeural
Russian	SvetlanaNeural
Spanish	ElviraNeural
Telugu	ShrutiNeural

Export to Sheets
Setup and Prerequisites
To run this application locally and connect it to your own Azure account, follow these setup instructions.

Azure Subscription: You must have an active Azure subscription.

Create an Azure Speech Resource: The text-to-speech avatar feature is a premium service and is only available in specific Azure regions. You must create your Speech resource in one of the following regions: West US 2, West Europe, or Southeast Asia.

Configure Environment Variables: You need to provide your Azure subscription key and service region to the application. This can be done by creating a .env file in the root of the project directory with the following content:

Code snippet

SUBSCRIPTION_KEY=&lt;your_subscription_key&gt;
SERVICE_REGION=&lt;your_service_region&gt;
Replace &lt;your_subscription_key&gt; and &lt;your_service_region&gt; with the actual credentials from your Azure Speech resource.

Potential Use Cases and Applications
This technology has wide-ranging applications across various industries, including:

Virtual Assistants and Chatbots: Enhance user interaction with lifelike virtual agents.

Corporate and Educational Training: Create engaging and scalable training modules and e-learning content.

Digital Content Creation: Automate the production of video content for news, presentations, and social media.

Accessibility: Develop advanced accessibility tools that provide information through a human-like interface.
