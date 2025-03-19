# Baking with the Gemini API

Note this is a fork of a google project.

A web application that analyzes images of baked goods using Google's Gemini Pro Vision multimodal model and generates recipes based on the image content.

![Baking App Demo](https://via.placeholder.com/800x400?text=Baking+App+Demo)

## 🧩 Overview

This project demonstrates how to use Google's Gemini Pro Vision API to analyze food images and generate corresponding recipes. The application features:

- Image selection from preloaded options
- Custom image upload capability
- Real-time recipe generation using the Gemini multimodal model
- Markdown rendering of recipe results

## 🛠️ Technologies Used

- [Google Gemini API](https://ai.google.dev/) - Google's multimodal AI model
- [LangChain.js](https://js.langchain.com/) - Framework for working with LLMs
- [Project IDX](https://idx.dev/) - Web-based development environment (optional)
- [Markdown-it](https://github.com/markdown-it/markdown-it) - Markdown parser for rendering results

## 🚀 Setup Instructions

### Prerequisites

- A Google Gemini API key (get one at [https://g.co/ai/idxGetGeminiKey](https://g.co/ai/idxGetGeminiKey))
- Node.js and npm installed on your system

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/baking-with-gemini.git
   cd baking-with-gemini
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the project root and add your Google API key:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:3000` (or the port specified in your console)

## 🔧 Project Structure

- `index.html` - Main HTML structure with image picker and form
- `main.js` - Core application logic, handles API calls to Gemini
- `style.css` - Styling for the application (imported in main.js)
- `gemini-api-banner.js` - Helper for API key validation notification

## 🖼️ Using the Application

1. Select one of the preloaded baked goods images or upload your own
2. The default prompt is "Provide a recipe for the baked goods in the image"
3. You can customize the prompt as needed
4. Click "Go" to generate a recipe based on the image
5. The recipe will appear in the results section, formatted as markdown

## 👩‍💻 Development with Project IDX

This project is compatible with [Project IDX](https://idx.dev/), Google's cloud-based development environment:

1. Visit [idx.dev](https://idx.dev/) and sign in with your Google account
2. Create a new project or open an existing one
3. Clone this repository into your IDX workspace
4. IDX will automatically detect and set up the project
5. Set your Gemini API key in the `.env` file
6. Use the built-in terminal to run `npm install` and `npm run dev`

## 📦 Deployment Options

### Vercel

1. Push your project to GitHub
2. Connect your repository to [Vercel](https://vercel.com/)
3. Configure environment variables (GOOGLE_API_KEY)
4. Deploy!

### Netlify

1. Push your project to GitHub
2. Connect your repository to [Netlify](https://netlify.com/)
3. Configure environment variables (GOOGLE_API_KEY)
4. Set build command and output directory based on your setup
5. Deploy!

### Google Cloud Run

1. Build a Docker container for your application
2. Push to Google Container Registry
3. Deploy as a Cloud Run service with your GOOGLE_API_KEY as an environment variable

## ⚠️ Important Notes

- This application handles API keys in the client side for demonstration purposes only
- For production use, consider implementing a backend proxy to handle API calls securely
- Ensure you comply with Google's Gemini API usage policies
- The application requires internet access to call the Gemini API

## 📄 License

[MIT](LICENSE)

## 🙏 Acknowledgements

- Google Gemini team for providing the API
- Project IDX team for the development environment
- All contributors to the open-source libraries used in this project