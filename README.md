<p align="center">
  <br/>
    <a href="https://pdf-redaction.com/" target="_blank"><img alt="PDF Redaction"
    src="https://pdf-redaction.com/images/pdf-redaction-logo.svg" width="450" style="max-width: 100%;"></a>
  <br/>
</p>

<p align="center">
    <i>Secure Your PDFs with AI-powered Redaction</i>
</p>

<p align="center">
    <a href="https://github.com/stabrise/spark-pdf/blob/main/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/stabrise/spark-pdf.svg?color=blue"></a>
    <a href="https://stabrise.com"><img alt="StabRise" src="https://img.shields.io/badge/powered%20by-StabRise-orange.svg?style=flat&colorA=E1523D&colorB=blue"/></a>
</p>

# PDF Redaction Studio: Self-Hosted Secure Document Redaction

PDF Redaction Studio is a powerful web-based application for redacting sensitive information from PDF documents. This is the backend container for the Studio edition.

<img src="https://raw.githubusercontent.com/StabRise/pdf-redaction-studio/main/images/pdf-redaction-studio.png" alt="PDF Redaction Studio Screenshot" height="300">


## Features

- **Professional PDF Redaction**: Advanced tools for redacting text, images, and metadata from PDFs
- **AI-Powered Detection**: Automatic detection of PII, sensitive data, and custom patterns
- **Custom Redaction Rules**: Define your own redaction patterns and rules
- **User-Friendly Interface**: Intuitive drag-and-drop interface built with React and Next.js
- **Real-time Preview**: See redactions in real-time before applying changes
- **Secure Processing**: All processing happens on your own infrastructure
- **Flexible Licensing**: Free trial available, with pay-as-you-go and subscription options

## Demo

You can try it out for free before start local installation at [https://studio.pdf-redaction.com](https://studio.pdf-redaction.com)

## Online Tool

For quick redaction online for free at [https://pdf-redaction.com](https://pdf-redaction.com)

## Pricing & Licensing

- **Free Trial**: Get started with a 14-days free trial to explore all features
- **Pay-as-you-go**: Flexible licensing option that scales with your usage
- **Subscription Plans**: Volume-based subscriptions for teams and enterprises

For detailed pricing information, visit [https://pdf-redaction.com/pricing/](https://pdf-redaction.com/pricing/)

Valid license key is required to start the service. You can obtain a free trial or a commercial license at [pdf-redaction.com](https://pdf-redaction.com/licenses/).

---

## 🛠 Quick Start

### 🚀 Instant Install self-hosted PDF Redaction Studio

 - Option A (curl): 
    ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/StabRise/pdf-redaction-studio/main/install.sh)"
    ```

 - Option B (wget): 
    ```bash
    /bin/bash -c "$(wget -qO- https://raw.githubusercontent.com/StabRise/pdf-redaction-studio/main/install.sh)"
    ```

### 🐳 Manual Installation with Docker Compose

If you prefer manual setup or want to customize the installation:

1. **Clone or download the repository files**:

   **Option A - Clone the repository:**
   ```bash
   git clone https://github.com/StabRise/pdf-redaction-studio.git
   cd pdf-redaction-studio
   ```

   **Option B - Download individual files:**
   ```bash
   mkdir pdf-redaction-studio && cd pdf-redaction-studio
   curl -O https://raw.githubusercontent.com/StabRise/pdf-redaction-studio/main/docker-compose.yaml
   curl -O https://raw.githubusercontent.com/StabRise/pdf-redaction-studio/main/.env.example
   ```

2. **Configure environment variables**:
   ```bash
   cp .env.example .env
   # Edit .env and add your license key from https://pdf-redaction.com/licenses/
   ```

3. **Start the services**:
   ```bash
   docker compose up -d
   ```

4. **Access the application**: Open http://localhost:3000 in your browser

**Useful Docker Compose commands:**
- `docker compose logs -f` - Follow logs in real-time
- `docker compose down` - Stop and remove containers
- `docker compose restart` - Restart the services
- `docker compose ps` - Show running containers

### 🐳 Docker Images

This project uses the following Docker images:

- **[postgres](https://hub.docker.com/_/postgres)** - Official PostgreSQL database image
- **[stabrise/pdf-redaction-studio-backend](https://hub.docker.com/r/stabrise/pdf-redaction-studio-backend)** - Backend API server
- **[stabrise/pdf-redaction-studio-frontend](https://hub.docker.com/r/stabrise/pdf-redaction-studio-frontend)** - Frontend web interface
- **[stabrise/pdf-redaction-api](https://hub.docker.com/r/stabrise/pdf-redaction-api)** - PDF Redaction API server

You can pull individual images separately:
```bash
docker pull stabrise/pdf-redaction-studio-backend:latest
docker pull stabrise/pdf-redaction-studio-frontend:latest
docker pull stabrise/pdf-redaction-api:latest
```

## Documentation

For full documentation, visit [https://pdf-redaction.com/docs/studio/](https://pdf-redaction.com/docs/studio/)

## Support

- **Website**: https://pdf-redaction.com
- **Documentation**: https://pdf-redaction.com/docs/studio/
- **Contact**: https://pdf-redaction.com/contact-us/
- **Email**: support@pdf-redaction.com

---