# Env Protector

![Made For VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)
![License](https://img.shields.io/github/license/sametcn99/env-protector.svg)
![Stars](https://img.shields.io/github/stars/sametcn99/env-protector.svg)
![Watchers](https://img.shields.io/github/watchers/sametcn99/env-protector.svg)
![Release](https://img.shields.io/github/release/sametcn99/env-protector.svg)
![Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/sametcn99.env-protector?label=VS%20Marketplace&logo=visual-studio-code)

![Banner](assets/banner.png)

## 🚀 Features

- **🔒 Toggle Visibility of Environment Files**: Easily toggle the visibility of environment files in the sidebar. This command modifies your workspace settings by adding `"**/.env*": true` to the `files.exclude` section in your `settings.json`.  
  ![Commands](assets/commands.png)
- **🛑 Confirmation Prompt Before Opening**: Prevent accidental exposure of sensitive data by receiving a confirmation prompt before opening an `.env` file. This safeguard adds an extra layer of security when handling critical environment variables.  
  ![Confirmation Dialog](assets/dialog.png)
- **🤐 Mask Sensitive Data**: Automatically mask sensitive environment variables when viewing `.env` files. Variable values are replaced with asterisks, allowing you to review the structure of the file without compromising the actual data.  
  ![Masked Variables](assets/masked.png)
- **➕ Add Environment Value Without Opening**: Insert new environment variables directly from the command palette without needing to open the `.env` file. This feature minimizes exposure risks while making it easy to update your environment.
  ![Add Environment Value](assets/add.gif)
- **✍️ Edit Environment Value Without Opening**: Quickly edit an existing environment variable from your enviroment files without exposing their contents in the editor.
  ![Edit Environment Value](assets/edit.gif)
- **➖ Remove Environment Value Without Opening**: Easily remove environment variables from your environment files, again without exposing their contents in the editor.
  ![Remove Environment Value](assets/remove.gif)

## 📦 Installation

You can install **Env Protector** either from the Visual Studio Code marketplace or manually using the steps below:

### Manual Installation

1. Download the `.vsix` file from the [releases page](https://github.com/sametcn99/env-protector/releases).
2. Open Visual Studio Code.
3. Navigate to the **Extensions** view by clicking the Extensions icon in the Activity Bar.
4. Click the ellipsis (...) in the top right corner of the Extensions view.
5. Select "Install from VSIX..." and choose the downloaded `.vsix` file.

## � Building from Source

If you want to build **Env Protector** from source, follow these steps:

### Prerequisites

- **Node.js** (version 14 or higher)
- **npm** (comes with Node.js)
- **Git**

### Build Steps

1. **Clone the repository**:

   ```bash
   git clone https://github.com/sametcn99/env-protector.git
   cd env-protector
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Compile the extension**:

   ```bash
   npm run compile
   ```

4. **Package the extension** (optional):

   ```bash
   npm run vsce
   ```

   This will create a `.vsix` file that you can install manually.

### Development Mode

For development and testing purposes, you can run the extension in watch mode:

```bash
npm run watch
```

This will automatically recompile the extension whenever you make changes to the source code.

#### Running with VS Code Run and Debug

You can also run and debug the extension directly within VS Code:

1. **Open the project in VS Code**:

   ```bash
   code .
   ```

2. **Start the watch task** (optional but recommended):
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
   - Type "Tasks: Run Task"
   - Select "npm: watch" to start automatic compilation

3. **Launch the Extension Development Host**:
   - Press `F5` or go to `Run and Debug` view (`Ctrl+Shift+D`)
   - Select "Run Extension" from the dropdown
   - Click the play button or press `F5`

This will open a new VS Code window (Extension Development Host) with your extension loaded. You can test all the extension features in this environment, and any changes you make to the code will be reflected after reloading the window (`Ctrl+R` in the Extension Development Host).

## �👥 Contributing

Contributions are highly welcome! If you'd like to help improve **Env Protector**, please follow these steps:

1. Fork the repository to your own GitHub account.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test them thoroughly.
4. Submit a pull request, describing your changes in detail.

Together, we can make **Env Protector** an even more valuable tool for the community!  
Thank you for your contributions!

## 📄 License

This project is licensed under the [GPL-3.0 license](LICENSE).
