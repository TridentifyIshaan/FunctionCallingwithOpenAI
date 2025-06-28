# Function Calling with OpenAI

A comprehensive Jupyter notebook demonstrating how to implement function calling with Azure OpenAI's GPT models. This project showcases how to create, configure, and execute custom functions that AI models can call to perform specific tasks.

## 🚀 Features

- **Function Calling Implementation**: Learn how to define and use custom functions with OpenAI's function calling API
- **Azure OpenAI Integration**: Complete setup and configuration for Azure OpenAI services
- **Real-world Examples**: Practical functions including:
  - Current time retrieval for different timezones
  - User preference queries (favorite color example)
- **Error Handling**: Robust error handling and validation
- **Interactive Learning**: Step-by-step Jupyter notebook format

## 📋 Prerequisites

Before running this project, make sure you have:

- Python 3.8 or higher
- Azure OpenAI account and API key
- Jupyter Notebook or VS Code with Jupyter extension

## 🛠️ Installation

1. Clone this repository:
```bash
git clone https://github.com/your-username/FunctionCallingwithOpenAI.git
cd FunctionCallingwithOpenAI
```

2. Install required packages:
```bash
pip install openai
```

## ⚙️ Configuration

### Azure OpenAI Setup

1. **Get your Azure OpenAI credentials**:
   - Azure OpenAI API Key
   - Azure OpenAI Endpoint URL
   - Deployment name for your model

2. **Update the configuration in the notebook**:
   - Replace `deployment_name` with your actual deployment name
   - Update the `azure_endpoint` with your Azure OpenAI endpoint
   - Set your `api_key`

### Environment Variables (Recommended)

For security, it's recommended to use environment variables:

```bash
export AZURE_OPENAI_API_KEY="your-api-key-here"
export AZURE_OPENAI_ENDPOINT="https://your-resource.openai.azure.com/"
export AZURE_OPENAI_DEPLOYMENT="your-deployment-name"
```

## 📖 Usage

1. **Open the Jupyter notebook**:
```bash
jupyter notebook 1.ipynb
```

2. **Run the cells sequentially**:
   - Start with package installation
   - Configure your Azure OpenAI settings
   - Execute the function definitions
   - Run the conversation example

3. **Customize the functions**:
   - Modify existing functions or add new ones
   - Update the function schemas in the `tools` array
   - Test with different user queries

## 🔧 Function Examples

### Current Time Function
```python
def get_current_time(location):
    """Get the current time for a given location"""
    # Returns current time for specified timezone
```

### Favorite Color Function
```python
def favorite_color():
    """Return user's favorite color"""
    # Returns predefined favorite color
```

## 📚 What You'll Learn

- How to define function schemas for OpenAI's function calling
- Proper JSON schema formatting for function parameters
- Handling function calls in OpenAI responses
- Error handling and validation
- Best practices for Azure OpenAI integration

## 🔍 Code Structure

```
FunctionCallingwithOpenAI/
├── 1.ipynb              # Main Jupyter notebook
├── README.md            # This file
└── .gitignore          # Git ignore file (recommended)
```

## 🚨 Troubleshooting

### Common Issues

1. **Connection Error**:
   - Verify your Azure OpenAI endpoint URL
   - Check your API key is valid
   - Ensure your deployment name is correct

2. **Function Not Called**:
   - Verify function schema matches your function definition
   - Check parameter types and requirements
   - Ensure function names are consistent

3. **API Version Issues**:
   - Use a stable API version (e.g., "2024-02-01")
   - Check Azure OpenAI documentation for latest versions

### Debug Tips

- Check the `response_message` to see what the model is trying to do
- Print function arguments to verify correct parsing
- Use try-catch blocks for better error handling

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Azure OpenAI team for the comprehensive API
- OpenAI for the function calling capabilities
- The Jupyter community for the excellent notebook environment

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Troubleshooting](#🚨-troubleshooting) section
2. Review the [Azure OpenAI documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/openai/)
3. Open an issue in this repository

---

**Happy Coding!** 🎉

Made with ❤️ for the AI development community