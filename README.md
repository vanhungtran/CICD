# GitLab CI/CD Masterclass Tutorial

🚀 **Interactive tutorial website for learning GitLab CI/CD concepts**

## 🌟 Features

- Interactive GitLab CI/CD tutorial
- Modern responsive design with Tailwind CSS
- Animated demonstrations and visual guides
- Comprehensive examples and best practices
- Resource gallery with workflow diagrams

## 🔧 CI/CD Pipeline

This project uses **GitHub Actions** for automated CI/CD with the following stages:

### 📋 Pipeline Stages

1. **Build & Test**
   - HTML validation
   - Link checking
   - Website startup testing
   - Artifact creation

2. **Security Scan**
   - Secret detection
   - File structure validation
   - Security best practices check

3. **Deploy**
   - Automatic deployment to GitHub Pages
   - Post-deployment verification
   - Live URL generation

4. **Notification**
   - Pipeline status reporting
   - Success/failure notifications

### 🚀 Automatic Deployment

- **Triggers**: Push to `main` branch
- **Target**: GitHub Pages
- **URL**: Auto-generated GitHub Pages URL
- **Files**: All HTML, MD, and resource files (excluding `main.js`)

## 🛠️ Local Development

### Prerequisites
- Node.js (v18+)
- Git

### Running Locally

```bash
# Clone the repository
git clone https://github.com/vanhungtran/CICD.git
cd CICD

# Start local development server
npx http-server -p 8000

# Open in browser
# http://localhost:8000
```

### Project Structure

```
CICD/
├── .github/workflows/     # GitHub Actions CI/CD
├── resourses/            # Images and diagrams
├── index.html            # Main tutorial page
├── tutorial.html         # Tutorial content
├── examples.html         # Code examples
├── docs.html            # Documentation
├── design.md            # Design specifications
├── interaction.md       # Interaction guidelines
├── outline.md           # Content outline
├── .gitignore           # Git ignore rules
└── README.md           # This file
```

## 🔄 CI/CD Workflow

### On Push to Main:
1. ✅ **Automated Testing** - HTML validation, link checking
2. 🔍 **Security Scanning** - Secret detection, structure validation  
3. 🚀 **Auto Deployment** - Deploy to GitHub Pages
4. 📊 **Status Reporting** - Pipeline results notification

### On Pull Request:
1. ✅ **Build & Test** - Validate changes
2. 🔍 **Security Scan** - Check for issues
3. 📝 **Status Check** - Required before merge

## 🌐 Live Website

The website is automatically deployed to GitHub Pages on every push to the main branch.

**Live URL**: [Will be available after first deployment]

## 📝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

The CI/CD pipeline will automatically test your changes!

## 🔧 Configuration

### GitHub Pages Setup Required:
1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
3. The workflow will handle the rest automatically

### Environment Variables:
- No additional environment variables required
- Uses GitHub's built-in `GITHUB_TOKEN` for deployments

## 📚 Learning Resources

This project demonstrates:
- GitHub Actions workflows
- Automated testing strategies
- Security scanning practices
- Continuous deployment patterns
- GitHub Pages integration

Perfect for learning modern CI/CD practices with GitHub! 🎓