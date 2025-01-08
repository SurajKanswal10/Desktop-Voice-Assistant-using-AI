#Desktop Voice Assistant using AI

OVERVIEW
This project is a desktop voice assistant that can perform various tasks like searching Wikipedia, opening websites, playing music, fetching the time, and sending emails through voice commands. The assistant listens to the user's commands using speech recognition and performs the corresponding task. It also utilizes text-to-speech (TTS) to speak back to the user.

FEATURES
Voice Command Recognition: It listens to the user and processes their commands.
Wikipedia Search: Allows the user to search Wikipedia and get a spoken summary.
Open Websites: Supports opening websites such as YouTube, Google, StackOverflow, etc.
Play Music: Plays music from a local directory of songs.
Get Current Time: Responds with the current time.
Open Applications: Opens applications like VS Code.
Send Emails: Can send emails using the user's Gmail account.

TECHNOLOGIES USED
Python: The core programming language used for the development of this voice assistant.
pyttsx3: For text-to-speech conversion.
SpeechRecognition: To recognize speech from the user's microphone.
wikipedia: For retrieving information from Wikipedia.
webbrowser: To open websites in a browser.
os: For accessing the system's local files and applications.
smtplib: For sending emails through Gmail.

REQUIREMENTS
Before running the code, make sure you have the following Python libraries installed:
pyttsx3
SpeechRecognition
wikipedia
webbrowser
os (Standard Python library)
smtplib (Standard Python library)

You can install the required libraries using the following pip commands:
bash
Copy code-
pip install pyttsx3
pip install SpeechRecognition
pip install wikipedia

SETUP INSTRUCTIONS
Clone or Download the repository: Download the source code to your local machine.
Install the dependencies: Use the commands above to install the required libraries.
Update Email Credentials: Before using the email functionality, replace the placeholders in the sendEmail function with your Gmail email and password:
python
Copy code-
server.login('youremail@gmail.com', 'your-password')
server.sendmail('youremail@gmail.com', to, content)
Make sure to enable "Less Secure Apps" or use an App Password if you have 2FA enabled on your Gmail account.
Run the Program: After the setup is complete, you can run the script. Simply execute the Python file in your terminal/command prompt:
bash
Copy code-
python voice_assistant.py

USAGE
Voice Commands: Once the program starts, it will greet you and listen for your commands. Example commands include:
"Search Wikipedia for <query>"
"Open YouTube"
"Play music"
"The time"
"Send an email to xyz@example.com"
Responding to Commands: The assistant will recognize the command and perform the corresponding action. For example, if you say "The time", it will respond with the current time.

Send Email: If you want to send an email, you can say "Email to xyz". It will ask you what to say and then send the email.

CODE FLOW
The assistant first greets the user and waits for a voice command.
It processes the command using the takeCommand() function and executes the corresponding action.
The assistant uses pyttsx3 for text-to-speech responses and speech_recognition to convert speech to text.
Commands related to opening applications or websites are handled via the os and webbrowser libraries.
If a Wikipedia search is triggered, it uses the wikipedia library to fetch information.
For sending emails, the smtplib library is used to interact with Gmail's SMTP server.

TROUBLESHOOTING
Voice Recognition Issue: Ensure that your microphone is set up properly and that you have granted permission to access it.
Email Sending Error: If emails are not sending, check if "Less Secure Apps" is enabled on your Gmail account or use an App password for authentication if 2FA is enabled.

Feel free to modify the content according to your specific needs or any additional features you have added!



