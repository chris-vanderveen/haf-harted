# Getting Started

## 1. Install Visual Studio Code

- Go to: https://code.visualstudio.com/
- Click "Download for Windows" and install.

## 2. Install Git

- Go to: https://git-scm.com/download/win
- Download and install Git for Windows (use default options).

## 3. Clone the Repository

- Open VS Code.
- Open the Command Palette (press `Ctrl+Shift+P`).
- Type "Git: Clone" and select it.
- Paste the repository URL (https://github.com/chris-vanderveen/haf-harted) and choose a folder to save it.
- When prompted, open the cloned folder in VS Code.

## 4. Export Your Blender Model

- In Blender, export your model as a `.glb` file.
- Avoid spaces in the file name (e.g., `myModel.glb`).

## 5. Add Your Model

- Place your `.glb` file inside the `public` folder of the project.

## 6. Update the Code

- In VS Code, open `main.js`.
- Find the line:
  ```
  loader.load(
    "YOUR FILE NAME HERE",
  ```
- Replace `"YOUR FILE NAME HERE"` with your file name, e.g. `"myModel.glb"`.

## 7. Install Node.js and npm

- Go to: https://nodejs.org/
- Download the LTS version for Windows and install.
- This will also install npm (Node Package Manager).

## 8. Open the Terminal in VS Code

- In VS Code, click "Terminal" in the top menu.
- Select "New Terminal".
- A terminal window will open at the bottom.

## 9. Install Dependencies

- Copy and paste these commands into the terminal, pressing Enter after each:
  ```
  npm install --save three
  npm install --save-dev vite
  ```

## 10. Start the Development Server

- In the terminal, run:
  ```
  npx vite
  ```
- You will see a message like:
  ```
  Local: http://localhost:5173/
  ```
- Click the link or copy it into your browser to view your scene.

---

If you have any issues, make sure your `.glb` file is in the `public` folder and the file name matches what you put in `main.js`.
