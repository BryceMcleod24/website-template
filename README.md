# 🌐 Standardized Website Project Template

## 📄 Description
This repository serves as a template for creating standardized web development projects. It includes a predefined project structure, configuration files, and deployment setup to ensure speed and consistency across projects.

## 🗂️ Project Structure

├── .github/              # GitHub Actions for auto-deploy
│   ├── workflows/
│       └── deploy.yml
├── admin/                # Decap CMS config.yml  
│   ├── config.yml        # For configuring Decap CMS
├── src/                  # Content, layouts, and static assets
│   ├── content/          # Markdown files for pages/blog posts  
│   ├── layouts/          # Hugo/Jekyll templates  
│   └── static/           # Images, CSS, JS
├── .gitignore            # Files and directories to be ignored by Git
├── LICENSE
├── netlify.toml          # Netlify deployment config  
└── README.md             # Project setup guide  

## ⚙️ Setup
1. **Clone the repository:**
    ```sh
    git clone https://github.com/BryceMcLeod24/website-template.git
    cd website-template
    ```

2. **Install dependencies:**
    ```sh
    npm install
    ```

3. **Start the development server:**
    ```sh
    npm start
    ```

## 🚀 Deployment
This project is configured to deploy to Netlify using GitHub Actions. On every push to the `main` branch, the site will be automatically deployed.

### 📚 Netlify Configuration
Ensure you have the following secrets set in your GitHub repository:
- `NETLIFY_AUTH_TOKEN`
- `NETLIFY_SITE_ID`

## Usage
1. **Update the [config.yml](http://_vscodecontentref_/6) file:**
    Replace the `repo` field with your GitHub repository details.
    ```yml
    backend:
      name: github
      repo: your-username/your-repo-name
      branch: main
    ```

2. **Customize the content:**
    Add or modify content in the [content](http://_vscodecontentref_/7) directory.

3. **Customize the layout:**
    Update the layout files in the [layouts](http://_vscodecontentref_/8) directory.

## 🤝 Contributing
Feel free to submit issues or pull requests if you find any bugs or have suggestions for improvements.

## 📜 License
This project is licensed under the MIT License.
