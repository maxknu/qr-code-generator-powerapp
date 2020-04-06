## Description
Simple Canvas PowerApp to generate QR code from a website. This example is meant to work with https://github.com/maxknu/azureqrcodeapp or any other qr code generator which returns an image

## Getting started
```bash
# 1. Go to PowerApps.com and login with your business account
#    Or create a community edition account https://powerapps.microsoft.com/sv-se/communityplan/
http://powerapps.com

# 2. On PowerApps.com, go to Apps => Import canvas app
PowerApps.com => Apps => Import canvas app

# 3. Upload App.zip provided in this repo. 
Upload App.zip 

# 4. Test the App, find it with name "qr-code-generator" in your Environment
Open qr-code-generator
```

## QR-Code generator dependency
This app depends on a QR Code generator which returns an image
you can point to your own or use https://github.com/maxknu/azureqrcodeapp

## modify qr-generator URL
```bash
# Inside the PowerApps Editor
Open QRScreen

# Select Image1 component
Select Image1

# Modify Image function in the codebar
Modify "https://qrcodeapp20.azurewebsites.net/?text="& Url.Text &"&size=10" & "&token=secrettoken" 
```