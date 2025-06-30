Handwritten Text Converter

This project is a web-based application that converts handwritten text from images into editable plain text, attempting to preserve the original line breaks and paragraph formatting. It leverages the power of the Google Cloud Vision API for Optical Character Recognition (OCR).
✨ Features

    Image Upload: Easily upload handwritten image files (PNG, JPG, etc.).

    Live Text Overlay: See the recognized text overlaid directly on your uploaded image, visually matching the original layout.

    Intelligent Line & Paragraph Detection: Utilizes advanced logic based on word bounding boxes to accurately reconstruct line breaks and paragraph spacing, mimicking your original notes.

    Smart Punctuation Handling: Ensures conventional spacing around punctuation marks (e.g., no space before periods, commas).

    Plain Text Preview: Review the extracted and formatted plain text directly in the browser before downloading.

    Text Download: Download the converted text as a .txt file, ready for use in any text editor.

    Responsive Design: A clean and responsive user interface built with Tailwind CSS, ensuring usability across different devices.

🚀 How to Use

    Clone the Repository:

    git clone <your-repo-url>
    cd handwritten-text-converter

    Open the Application:
    Open the index.html file directly in your web browser.

    open index.html
    # or start a simple local server (recommended for development)
    python3 -m http.server

    Get Your Google Cloud Vision API Key:
    Follow the instructions in the "How to Get a Google Cloud Vision API Key" section below.

    Insert Your API Key:
    Open the index.html file in a text editor. Locate the JavaScript section and find the line:

    const VISION_API_KEY = ''; // YOUR_API_KEY_HERE

    Replace '' with your actual Google Cloud Vision API Key.

    Upload an Image: Click the "Upload Handwritten Image" button and select an image file containing handwritten text.

    Convert to Text: Click the "Convert to Text" button. The application will process the image and display the recognized text.

    Review and Download: Review the converted text in the preview area. If satisfied, click the "Download Text" button to save it as a .txt file.

🔑 How to Get a Google Cloud Vision API Key

To use this application, you need an API key from Google Cloud Platform with the Cloud Vision API enabled.

    Go to Google Cloud Console: Navigate to the Google Cloud Console.

    Create a New Project (or select an existing one):

        Click on the project selector dropdown at the top.

        Click "New Project" and follow the prompts to create a new project.

        If you have an existing project, select it.

    Enable the Cloud Vision API:

        In the Google Cloud Console, use the navigation menu (☰) on the left.

        Go to APIs & Services > Library.

        Search for "Cloud Vision API" and select it.

        Click the "Enable" button.

    Create API Credentials:

        In the Google Cloud Console, go to APIs & Services > Credentials.

        Click "+ CREATE CREDENTIALS" at the top and select "API key".

        Your API key will be generated. Copy this key.

        Important: For client-side applications like this one, it's highly recommended to restrict your API key to prevent unauthorized use.

            Click "RESTRICT KEY" on the API key details page.

            Under "Application restrictions," select "HTTP referrers (web sites)" and add your domain(s) (e.g., http://localhost:8000/* for local testing, or your deployed website's URL).

            Under "API restrictions," select "Restrict key" and choose "Cloud Vision API" from the dropdown.

            Click "Save".

🛠️ Technologies Used

    HTML5: For the application structure.

    CSS3 (Tailwind CSS): For responsive and modern styling.

    JavaScript (ES6+): For application logic and API interaction.

    Google Cloud Vision API: The core OCR engine for text recognition and layout analysis.

🤝 Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please feel free to:

    Fork the repository.

    Create a new branch (git checkout -b feature/your-feature-name).

    Make your changes.

    Commit your changes (git commit -m 'Add new feature').

    Push to the branch (git push origin feature/your-feature-name).

    Open a Pull Request.

📄 License

This project is open-sourced under the MIT License. See the LICENSE file for more details.