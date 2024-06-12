
# Discord Token Login Script

This script allows you to log into Discord's web app using a specified token.

**Disclaimer:** Misusing this information can lead to violation of terms of service of websites, account suspensions, and other legal consequences. Use this knowledge responsibly and ethically.

## Step 1: Prepare the JavaScript Code

1. **Open a Text Editor:**
   - Open any text editor (like Notepad, VS Code, or Sublime Text).

2. **Copy the Following Script:**

   ```javascript
   function login(token) {
       setInterval(() => {
           document.body.appendChild(document.createElement`iframe`).contentWindow.localStorage.token = `"${token}"`;
       }, 50);
       setTimeout(() => { location.reload(); }, 2500);
   }
   login('TOKEN');
   ```

3. **Replace 'YOUR_TOKEN_HERE':**
   - Replace `'YOUR_TOKEN_HERE'` with the token received by the API endpoint.

## Usage Instructions

### Step 2: Execute the Script

1. **Go to Discord's Web App:**
   - Navigate to [Discord](https://discord.com) in your browser.

2. **Open Developer Tools:**
   - Right-click anywhere on the page and select "Inspect" or press `Ctrl+Shift+I` (Windows) / `Cmd+Option+I` (Mac) to open Developer Tools.

3. **Go to the Console Tab:**
   - In Developer Tools, go to the "Console" tab.

4. **Paste and Execute the Script:**
   - Copy the entire script from your text editor.
   - Paste it into the Console in Developer Tools and press `Enter`.

### Step 3: Wait and Observe

- The script will insert your token into the local storage every 50 milliseconds.
- After 2.5 seconds, the page will reload.
- You should be logged into Discord with the provided token.
- Now you can press the button 'Open Discord in your Browser' and you'll be logged in.

**Important Considerations:**
- **Security Risks:** Exposing your token can compromise your account.
- **Ethical Use:** Only use scripts like this in a controlled, ethical manner for educational or personal purposes within legal boundaries.
- **Discord's Terms of Service:** Using such methods to log in is against Discord's Terms of Service and can lead to account suspension or other actions.
