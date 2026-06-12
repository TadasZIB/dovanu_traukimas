# 🎁 Complete Beginner's Guide - Launch Frontend on Windows/Mac/Linux

This guide assumes **zero prior experience** with development. We'll go step-by-step!

---

## 📖 Part 1: Install Node.js (The Foundation)

Node.js is software that lets your computer run React code. Think of it like installing Adobe Photoshop, but for code.

### **For Windows:**

1. Go to https://nodejs.org/
2. You'll see two big buttons. Click the **LTS** button (green, left side)
   - LTS = "Long Term Support" (stable, tested version)
3. A file called `node-vXX.XX.X.msi` will download (might take 30 seconds)
4. **Double-click** the downloaded file
5. Click "Yes" when it asks "Do you want to allow this app to make changes?"
6. Click "Next" → "I Agree" → "Next" → "Next" → "Next" → **"Install"**
7. Wait for installation (takes 1-2 minutes)
8. Click **"Finish"**

### **For Mac:**

1. Go to https://nodejs.org/
2. Click the **LTS** button (green)
3. A file called `node-vXX.XX.X.pkg` will download
4. **Double-click** the downloaded file
5. Click "Continue" → "Agree" → "Continue" → "Install"
6. Enter your Mac password when asked
7. Wait for installation
8. Click **"Close"**

### **For Linux (Ubuntu/Debian):**

Open Terminal and copy-paste this:
```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt-get install -y nodejs
```

---

## ✅ Verify Installation

**This checks that Node.js installed correctly.**

### **For Windows, Mac, or Linux:**

1. Open **Command Prompt** (Windows) or **Terminal** (Mac/Linux)
   - **Windows**: Press `Win + R`, type `cmd`, press Enter
   - **Mac**: Press `Cmd + Space`, type `terminal`, press Enter
   - **Linux**: Press `Ctrl + Alt + T`

2. Type this command (then press Enter):
   ```
   node --version
   ```

3. You should see something like: `v18.16.0`

4. Type this command (then press Enter):
   ```
   npm --version
   ```

5. You should see something like: `9.6.7`

**If you see version numbers → Node.js installed successfully! ✅**

---

## 🔽 Part 2: Download the Project Code

Now we'll get the project code onto your computer.

### **Option A: Using Git (Recommended for Developers)**

1. Install Git from https://git-scm.com/
2. Open Command Prompt / Terminal
3. Go to a folder where you want to keep projects. For example:
   ```
   cd C:\Users\YourName\Documents
   ```
   (Replace `YourName` with your actual username)

4. Copy the project:
   ```
   git clone https://github.com/TadasZIB/Dovanu_traukimas.git
   ```

5. Go into the project folder:
   ```
   cd Dovanu_traukimas
   ```

### **Option B: Download as Zip (Easier for Beginners)**

1. Go to: https://github.com/TadasZIB/Dovanu_traukimas
2. Click the green **"Code"** button (top right)
3. Click **"Download ZIP"**
4. A file called `Dovanu_traukimas-main.zip` downloads
5. **Right-click** the zip file → **"Extract All"** (Windows) or **Double-click** (Mac)
6. You now have a folder called `Dovanu_traukimas-main`
7. Open Command Prompt/Terminal
8. Go into that folder. For example:
   ```
   cd C:\Users\YourName\Downloads\Dovanu_traukimas-main
   ```

---

## 📦 Part 3: Install Project Dependencies

Dependencies are like "plugins" or "add-ons" that the project needs to run.

1. **Make sure you're in the project folder.** Your Command Prompt/Terminal should show something like:
   ```
   C:\Users\YourName\Downloads\Dovanu_traukimas-main>
   ```
   or
   ```
   /Users/YourName/Dovanu_traukimas-main $
   ```

2. Go into the frontend folder:
   ```
   cd frontend
   ```

3. Now your path should show `frontend` at the end

4. Install dependencies by typing:
   ```
   npm install
   ```

5. **This will take 2-5 minutes.** You'll see lots of text scrolling past. This is normal! ✓

6. When it finishes, you'll see:
   ```
   added XXX packages, and audited XXX packages in XXm
   ```

**If you see that message → Installation successful! ✅**

---

## 🚀 Part 4: Start the App

Now for the exciting part - launching the app!

1. **Make sure you're still in the `frontend` folder.** Your terminal should show something ending in `frontend`

2. Type this command:
   ```
   npm start
   ```

3. **Wait 10-20 seconds...** The terminal will show:
   ```
   Compiled successfully!
   
   You can now view dovanu-traukimas-frontend in the browser.
   
     Local:            http://localhost:3000
   ```

4. **A browser window automatically opens!** 🎉

5. You should see:
   - A pink/turquoise gradient background
   - A big gift emoji 🎁 bouncing
   - "Who's Drawing Today?" title
   - A form to enter your name

---

## 🎮 Part 5: Test the App

Try clicking around! Here's what you can do:

1. **Enter a name** in the text field (or click "Choose from List")
2. Click **"Ready to Draw! 🎉"**
3. Click any of the 8 cards
4. The card flips and shows a gift! 🎁
5. Enter an email address
6. Click **"Send Result"**
7. See the success message with a joke! 😄
8. Click **"Back to Home"** to try again

---

## 🛑 Part 6: Stop the App

When you're done:

1. Go back to your **Command Prompt / Terminal**
2. Press **`Ctrl + C`** (hold Ctrl, press C)
3. It will ask: "Terminate batch job (Y/N)?" (Windows) or just exit
4. Type **`Y`** and press Enter (Windows only)
5. The app stops running and the browser page won't work anymore (that's normal)

---

## 🔄 Part 7: Run It Again Later

If you close everything and want to run it again:

1. Open Command Prompt / Terminal
2. Go to the project folder:
   ```
   cd C:\Users\YourName\Downloads\Dovanu_traukimas-main\frontend
   ```
3. Type:
   ```
   npm start
   ```
4. App launches again! 🚀

**You don't need to run `npm install` again - only the first time!**

---

## 🐛 Troubleshooting

### **Problem: "Command not found: npm"**
- **Solution**: Node.js didn't install. Go back to Part 1 and reinstall.

### **Problem: "Port 3000 already in use"**
- **Solution**: Another app is using port 3000. Try this:
  ```
  PORT=3001 npm start
  ```
  Then open http://localhost:3001 instead

### **Problem: "npm ERR! code EACCES"**
- **Solution**: Permissions issue. Try:
  ```
  sudo npm install -g npm
  ```

### **Problem: Blank white page or errors in browser**
- **Solution**: 
  1. Press `F12` to open Developer Tools
  2. Look for red error messages
  3. Copy the error and ask for help

### **Problem: Terminal says "npm is not recognized"**
- **Solution**: Node.js path not set. 
  1. Restart Command Prompt / Terminal
  2. If still doesn't work, reinstall Node.js

---

## 📁 Folder Structure Explained

```
Dovanu_traukimas/                    ← Main project folder
│
├── frontend/                        ← The React app (THIS ONE WE RUN)
│   ├── node_modules/               ← 400+ packages (don't touch!)
│   ├── public/                      ← HTML template
│   ├── src/                         ← All the app code
│   │   ├── pages/                  ← The 3 pages (Identification, Drawing, History)
│   │   ├── context/                ← User data storage
│   │   ├── styles/                 ← Colors, fonts, animations
│   │   ├── App.js                  ← Main app file
│   │   └── index.js                ← Startup file
│   ├── package.json                ← List of packages needed
│   └── .env.example                ← Configuration template
│
├── backend/                         ← Python stuff (for later phases)
├── README.md                        ← Project description
└── QUICKSTART.md                    ← Another quick guide
```

---

## 💡 Making Changes to the Code

**Want to modify something?** Here's how:

1. **Stop the app** (Ctrl + C in terminal)
2. Open the code file with any text editor (Notepad, VS Code, etc.)
   - Example: `frontend/src/pages/IdentificationPage.jsx`
3. Make your changes
4. **Save the file**
5. Go back to terminal, type `npm start`
6. The app **automatically refreshes** in your browser!

---

## 🎓 Learning Tips

- **Don't worry if you see errors** - they're learning opportunities!
- **Read the error messages** - they usually tell you what's wrong
- **Google is your friend** - most errors have solutions online
- **Ask questions** - no such thing as a silly question!

---

## ✨ Next Steps

Once you're comfortable running the app:

1. **Explore the code** - Look at what's in `src/pages/`
2. **Change colors** - Edit `src/styles/globals.css`
3. **Modify text** - Change the greeting in `IdentificationPage.jsx`
4. **Add your own cards** - Edit the drawing options in `DrawingPage.jsx`

---

## 📞 Need Help?

If you get stuck:
1. **Take a screenshot** of the error
2. **Copy the exact error message**
3. **Note what step you were on**
4. Ask for help!

---

**Happy coding! 🎁🎉**
