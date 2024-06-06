# trivy-installation

# on Linux distro

sudo apt-get install wget apt-transport-https gnupg lsb-release
wget -qO - https://aquasecurity.github.io/trivy-repo/deb/public.key | sudo apt-key add -
echo deb https://aquasecurity.github.io/trivy-repo/deb $(lsb_release -sc) main | sudo tee -a /etc/apt/sources.list.d/trivy.list
sudo apt-get update
sudo apt-get install trivy


# on Windows distro 
 choco install trivy -y
 choco upgrade trivy -y
choco uninstall trivy -y

# Usage

1. **Install Trivy:** Follow the installation instructions on the official Trivy website (search online for "Trivy installation").
2. **Scan an image:** Use the `trivy image <image_name>` command, replacing `<image_name>` with the actual name of the image you want to scan.
