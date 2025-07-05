# 🖼️ Azure Vision Chat App

A powerful Streamlit web application that enables interactive conversations about images using Azure AI/OpenAI vision models. Upload any image URL and ask questions to get detailed AI-powered analysis and insights.



## ✨ Features

### 🔍 **Image Analysis**
- **Dynamic Image Input**: Load any publicly accessible image via URL
- **Real-time Preview**: Instant image validation and display
- **Multi-format Support**: JPG, PNG, GIF, WebP images
- **Smart Format Detection**: Automatic MIME type detection

### 💬 **Interactive Chat**
- **One-click Questions**: Pre-built suggestion buttons for common queries
- **Custom Questions**: Type your own questions about the image
- **AI-Powered Responses**: Detailed analysis using Azure OpenAI/Foundry models
- **Error Handling**: Graceful error messages and validation

### 🎯 **Quick Question Categories**
- 🔍 **General Analysis**: "What do you see in this image?"
- 📝 **Detailed Description**: Comprehensive image overview
- 🎨 **Colors & Composition**: Visual design analysis
- 🌟 **Notable Features**: Interesting details and highlights
- 😊 **Mood & Atmosphere**: Emotional tone assessment
- 🏷️ **Object Identification**: Recognition and listing of subjects

### 🖼️ **Sample Images**
- 🍊 **Orange**: Default demo image
- 🏞️ **Landscape**: Nature photography from Unsplash
- 🐱 **Cat**: Animal photography examples

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Azure AI/OpenAI account with vision model access
- Streamlit

### Installation

1. **Clone or download the project files**
2. **Install dependencies**:
   ```bash
   pip install streamlit azure-identity azure-ai-projects
   ```

3. **Configure secrets** - Create `.streamlit/secrets.toml`:
   ```toml
   MODEL_DEPLOYMENT = "your-model-name"
   PROJECT_CONNECTION = "your-azure-endpoint-url"
   ```

4. **Run the application**:
   ```bash
   streamlit run chat-app.py
   ```

## 📁 Project Structure

```
├── chat-app.py              # Main Azure Vision Chat application
├── .streamlit/
│   └── secrets.toml        # Configuration secrets
└── README.md               # This file
```

## 🔧 Configuration

### Required Secrets
Configure these values in `.streamlit/secrets.toml`:

| Key | Description | Example |
|-----|-------------|---------|
| `MODEL_DEPLOYMENT` | Azure AI model name | `"Phi-4-multimodal-instruct"` |
| `PROJECT_CONNECTION` | Azure AI endpoint URL | `"https://your-endpoint.services.ai.azure.com/models"` |

### Azure Setup
1. **Create Azure AI Foundry resource** 
2. **Deploy a vision-capable model** (e.g., GPT-4 Vision, Phi-4 multimodal)
3. **Get endpoint URL and model name** from Azure AI Foundry portal
4. **Configure authentication** (Azure CLI login or managed identity)

## 🎮 How to Use

### Basic Workflow
1. **Enter Image URL**: Paste any public image URL
2. **Preview Image**: Verify the image loads correctly
3. **Choose Question**: Click a suggestion button or type custom question
4. **Get AI Response**: Click "Ask AI" for detailed analysis

### Sample Images
Click the sample image buttons to quickly test with different image types:
- **🍊 Orange**: Food/object analysis
- **🏞️ Landscape**: Nature scene description
- **🐱 Cat**: Animal identification

### Question Examples
- **General**: "What do you see in this image?"
- **Specific**: "How many people are in this photo?"
- **Creative**: "What story does this image tell?"
- **Technical**: "What's the lighting setup in this image?"

## 🛠️ Additional Apps

### Basic App (`basic_app.py`)
Simple Streamlit demo showing:
- Secret configuration reading
- Basic user interactions
- Azure connection status

### Web App (`web_app.py`)
Multi-page application featuring:
- **Home Dashboard**: Metrics and quick actions
- **Data Dashboard**: Charts and analytics
- **Web Tools**: URL checker, JSON formatter, text tools
- **Calculator**: Basic math and unit conversion
- **Contact Form**: Demo form with validation

## 🔒 Security Notes

- **Secrets Management**: Never commit secrets to version control
- **Image URLs**: Only use publicly accessible images
- **Azure Authentication**: Uses DefaultAzureCredential for secure access
- **Rate Limits**: Be mindful of Azure API usage limits

## 🐛 Troubleshooting

### Common Issues

**Image won't load:**
- Verify URL is publicly accessible
- Check image format (JPG, PNG, GIF, WebP)
- Ensure URL points directly to image file

**AI responses fail:**
- Check Azure endpoint configuration
- Verify model deployment name
- Confirm Azure authentication is working
- Check Azure subscription quota/limits

**Streamlit errors:**
- Ensure all dependencies are installed
- Check Python version compatibility
- Verify secrets.toml file location and format

### Debug Mode
Add to your secrets.toml for verbose logging:
```toml
debug = true
```

## 📚 Resources

- **[Streamlit Documentation](https://docs.streamlit.io/)**
- **[Azure AI Services](https://docs.microsoft.com/azure/cognitive-services/)**
- **[Azure OpenAI](https://docs.microsoft.com/azure/cognitive-services/openai/)**
- **[Unsplash](https://unsplash.com)** - Free stock photos
- **[Pexels](https://pexels.com)** - Free stock images

## 🤝 Contributing

Feel free to:
- Report bugs or issues
- Suggest new features
- Submit improvements
- Add more sample questions

## 📄 License

This project is provided as-is for educational and demonstration purposes.

## 🏷️ Version

**Current Version**: 1.0.0  
**Last Updated**: July 2025  
**Compatibility**: Python 3.8+, Streamlit 1.28+

---

Made with ❤️ using **Streamlit** and **Azure AI** 🚀

