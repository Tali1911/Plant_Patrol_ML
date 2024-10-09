# Plant_Patrol_ML
# WhatsApp Plant Disease Prediction Bot

## Project Overview
This project implements a WhatsApp bot that uses machine learning to predict plant diseases from images. Users can send a photo of a plant to the bot via WhatsApp, and the bot will analyze the image and respond with a prediction of any diseases affecting the plant.

## Key Features
- Integration with WhatsApp using Twilio's API
- Image processing and analysis using a pre-trained Keras model
- Real-time response with disease predictions
- Easy-to-use interface through WhatsApp
- Capability to identify 2197 different plant diseases

## Technical Stack
- Python 3.8+
- Flask for the web application framework
- Keras for loading and using the machine learning model
- Twilio API for WhatsApp integration
- Pillow (PIL) for image processing
- NumPy for numerical operations

## How It Works
1. A user sends a photo to the WhatsApp bot
2. Twilio forwards the message to our Flask application
3. The application downloads and preprocesses the image
4. The preprocessed image is fed into the Keras model for prediction
5. The prediction result is sent back to the user via WhatsApp

## Setup and Installation
1. Clone this repository
2. Install the required dependencies: `pip install -r requirements.txt`
3. Set up a Twilio account and configure the WhatsApp sandbox
4. Update the configuration file with your Twilio credentials
5. Run the Flask application: `python app.py`

## Usage
1. Add the Twilio WhatsApp sandbox number to your contacts
2. Send a message to the sandbox number to connect
3. Send a clear photo of a plant leaf to get a disease prediction

## Model Information
The plant disease prediction model was trained on the plant_diseases dataset using Keras. It can currently identify 2197 different plant diseases across various plant species.

## Future Enhancements
- Expand the model to cover more plant species and diseases
- Implement multi-language support
- Add detailed disease information and treatment recommendations

## Contributing
We welcome contributions! Please see our [CONTRIBUTING.md](link-to-contributing-file) for details on how to get started.

## License
This project is licensed under the [choose appropriate license] License - see the [LICENSE.md](link-to-license-file) file for details.

## Acknowledgments
- Twilio for providing the WhatsApp Business API
- The creators and maintainers of the plant_diseases dataset
