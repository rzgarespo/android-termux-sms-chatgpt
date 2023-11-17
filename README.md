
# Termux SMS ChatGPT Assistant

Termux SMS ChatGPT Assistant is a Python script that integrates with Termux on Android to automate the processing of SMS messages using OpenAI's GPT-3.5-turbo. The script listens for new SMS messages, analyzes their content, and generates responses using the OpenAI language model if the message ends with a question mark or any other symbols configured in the 'bodyIncludeText = "?"'.

## Features

- Listens for new SMS messages at regular intervals.
- Analyzes SMS content and generates responses using OpenAI GPT-3.5-turbo.
- Marks processed SMS as read to avoid repeated processing.
- Handles cases where 'sender' information is not available by using the 'number' field.

## Prerequisites

- Termux installed on an Android device.
- OpenAI GPT-3.5-turbo API key.
- Python installed on Termux.

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/rzgarespo/android-termux-sms-chatgpt.git
   ```

2. Navigate to the project directory:

   ```bash
   cd android-termux-sms-chatgpt
   chmod +x sms.py
   ```

3. Install the required Python packages:

   ```bash
   pkg install python
   pip install openai
   ```

4. Set up your OpenAI API key by replacing `"your-api-key"` in the script with your actual API key.

5. Run the script:

   ```bash
   python sms.py
   ```

## Configuration

- Adjust the script's configuration parameters, such as the API key, polling interval, and message processing logic, according to your preferences.

## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Termux](https://termux.com/)
- [OpenAI GPT-3.5-turbo](https://platform.openai.com/api-keys)

Feel free to contribute to the project or submit issues if you encounter any problems.

## Screenshot
![Screenshot](https://github.com/rzgarespo/android-termux-sms-chatgpt/raw/main/Screenshot.png)
