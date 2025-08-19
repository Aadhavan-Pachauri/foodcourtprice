# Food Court Pricing System

An AI-powered menu and cost analysis tool for food court pricing.

## Setup Instructions

### 1. Google AI API Key Configuration

To use the AI-powered ingredient estimation feature, you need to set up a Google Generative Language API key:

1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Open `config.js` and replace `YOUR_API_KEY_HERE` with your actual API key:
   ```javascript
   const API_CONFIG = {
     apiKey: 'your-actual-api-key-here',
     model: 'gemini-pro',
     baseUrl: 'https://generativelanguage.googleapis.com/v1beta/models'
   };
   ```

### 2. Running the Application

The application runs entirely in the browser. You can:
- Open `index.html` directly in your browser
- Or serve it locally using a simple HTTP server:
  ```bash
  python3 -m http.server 8000
  ```
  Then visit `http://localhost:8000`

## Features

- **Manual ingredient input** with quantity and pricing
- **AI-powered ingredient estimation** (requires API key)
- **Platform-specific pricing** (Society, Zomato, Swiggy)
- **Unique feature premiums** (+5% per feature)
- **Profit margin calculation**
- **Real-time price updates**

## File Structure

- `index.html` - Main application file
- `config.js` - API configuration (edit this for your API key)
- `README.md` - This documentation file

## Usage

1. Enter a dish name
2. Add ingredients manually or use "Auto-estimate Ingredients" (requires API key)
3. Select your platform (Society, Zomato, or Swiggy)
4. Choose unique features if applicable
5. Set your desired profit margin
6. View calculated pricing in real-time