### Project Overview

#### Purpose
This project is designed for users who want to run Ansible locally without the need to install any virtual machines or perform complex configurations.

#### Benefits
- **Simplified Setup:** Quickly set up an Ansible lab environment.
- **Ease of Use:** No need for VM installations or extensive configurations.

### Prerequisites

Before cloning and running the project, ensure Docker is installed on your local machine. Follow these steps:

#### Install Docker

1. **Visit the Docker Website:**
   Go to [docker.com](https://www.docker.com/get-started) to download Docker.

2. **Choose Your OS:**
   Select the appropriate Docker version for your operating system (Windows, macOS, or Linux).

3. **Download Docker:**
   Click the download link and follow the on-screen instructions to download the Docker installer.

4. **Install Docker:**
   - **Windows:**
     - Run the Docker installer.
     - Follow the installation wizard steps.
     - Ensure you check the option to use WSL 2 (Windows Subsystem for Linux) during installation.
   - **macOS:**
     - Open the downloaded `.dmg` file.
     - Drag the Docker icon to the Applications folder.
   - **Linux:**
     - Follow the specific instructions for your Linux distribution on the Docker website.

5. **Verify Installation:**
   Open your terminal or command prompt and run the following command to verify Docker is installed correctly:
    bash >> docker --version

### Example:
```bash
docker --version
# Output: Docker version 20.10.7, build f0df350
```
Note - Ensure Docker is running before proceeding to clone and run the Ansible project.