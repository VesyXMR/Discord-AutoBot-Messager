# Discord Auto-Messenger Bot
This bot automates sending messages in a Discord channel. It reads the contents of a messages.txt file (each line representing one message) and uses configuration information stored in an info.txt file (containing User ID, Discord token, channel URL, and channel ID) to connect to the channel. Additionally, the bot provides an external configuration menu to edit these files using a text editor.

Telegram Channel: https://t.me/cybinscrips_vesyxmr

Important:

This bot uses your user token to automate sending messages. Use it for testing purposes or with authorized accounts only, as using user tokens may violate Discord's Terms of Service.
Never share your tokens or credentials publicly!

# Requirements
Operating System: Windows (the .exe is compiled for Windows)
Embedded Files: The executable includes the info.txt and messages.txt files.
Executable: The compiled file (e.g., vesyxmr_bot.exe)
Optional: A text editor (e.g., Notepad on Windows) for editing configuration files

# Configuration Files
The bot uses two configuration files:

info.txt – Should contain four lines:

Line 1: User ID
Line 2: Discord token
Line 3: Discord channel URL
Line 4: Discord channel ID
messages.txt – Each line corresponds to a message that the bot will send.

Note:
If you wish to edit these files within the bot, a configuration menu is provided that opens your default text editor. Remember to save and close the text editor after making changes. If you close the editor without saving, a red warning message ("No changes made. (File content is the same)") will appear.

# Step-by-Step Usage

Login & Setup Developer Mode on Discord:

Login: Open your browser and log in with your Discord account.
Enable Developer Mode:
Go to Discord’s User Settings > Advanced and enable Developer Mode.

![422924256-739dd906-1a16-4624-a190-45e4708cf329](https://github.com/user-attachments/assets/9864c67d-ae87-489d-80d4-5a19707ba93e)


After that, execute the bot (the .exe file). When prompted with the configuration menu, select [1] Edit info.txt.
The bot will open the info.txt file in your default text editor.
Collect and Enter the Required Information:

## User ID:
Click on your profile picture in Discord and select “Copy ID”. Paste the copied User ID into the first line of the info.txt file.

![422924114-8429eb70-1ef2-4618-b1ca-a5665f5e8127](https://github.com/user-attachments/assets/0772b234-6577-475b-9c04-e72daf2e99a7)


## Discord token: 
Open the Developer Tools (Ctrl + Shift + I) in your browser, go to the Network tab, then send a message in your channel.
Look for a request that includes "messages" and check the Authorization header. Copy this token and paste it into the second line of info.txt.

![422923519-8215d46f-32c8-4ae2-a3bc-2b29d352fcb7](https://github.com/user-attachments/assets/348ee464-7a3b-4612-82dc-abbb7149b02a)


## Discord Channel URL
Copy the URL from your browser’s address bar while you are in the desired channel, and paste it into the third line.

![422925069-7419d445-1673-4bf3-bd72-b6cdeb298d81](https://github.com/user-attachments/assets/fed38361-5cba-4d1b-bf3c-a49700e7025b)


## Discord Channel ID
Right-click on the channel name in Discord and select “Copy Channel ID”. Paste the Channel ID into the fourth line.

![422925435-d1b49b16-5db4-4a26-8319-e8b2bb1318fa](https://github.com/user-attachments/assets/b4097b53-31d3-4756-a0d6-23d05382aa38)


Save and close the text editor after you have made the changes.

After all, you info.txt should be like this:

![image](https://github.com/user-attachments/assets/2a7d5fb0-a1b0-41a1-84b9-0d31ecd82669)

# Editing messages.txt:

Each line in messages.txt corresponds to one message that the bot will send.
To edit it, select [2] Edit messages.txt in the configuration menu.
Remember: After editing, save and close the text editor.
If you close without saving, the bot will show a red message stating, “No changes made. (File content is the same)”.

# Run the Bot

- Open a Command Prompt (CMD or PowerShell).
- Navigate to the directory where the .exe is located.
- Execute the bot by typing:
    ```bash 
    vesyxmr_bot.exe

The bot will display initial banners and prompt you to choose a language (English or Portuguese). Select the desired option.

# During Execution

The bot will read messages from messages.txt and send them to the specified Discord channel based on the settings in info.txt.
While running, if you want to stop the bot and return to the menu, a red message will instruct you to press a key (or Enter) to interrupt the bot.
To completely stop the bot, follow the on-screen instructions (or use CTRL+C if needed).
Logs and Output

The bot prints log messages with timestamps indicating when messages are sent, delays between messages, and any errors encountered.

# Additional Notes
Security: Keep your tokens and configuration files secure.
Selector Adjustments: If Discord’s or the text editor's interface changes, you might need to update the CSS selectors in the script.
Customization: You can change texts, colors, and banners directly in the source code before compiling the executable.
