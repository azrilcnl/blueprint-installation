# blueprint-installation
blueprint is an add-on for pterodactyl so you can install a theme very easily


# Installation
1. You must install the blueprint first
2. blueprint installation
```
nvm install 20
```
```
npm i -g yarn
```
```
cd /var/www/pterodactyl
```
```
yarn
```
```
apt install -y zip unzip git curl wget
```
```
wget "$(curl -s https://api.github.com/repos/BlueprintFramework/framework/releases/latest | grep 'browser_download_url' | cut -d '"' -f 4)" -O release.zip
```
```
unzip release.zip
```
```
touch /var/www/pterodactyl/.blueprintrc
```
```
echo \
'WEBUSER="www-data";
OWNERSHIP="www-data:www-data";
USERSHELL="/bin/bash";' >> /var/www/pterodactyl/.blueprintrc
```
```
chmod +x blueprint.sh
```
```
bash blueprint.sh
```
3. you are done
