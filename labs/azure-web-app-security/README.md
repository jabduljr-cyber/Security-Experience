# Azure Web App and Cloud Security (Bootcamp Project 1)

In this project I built and hosted a personal blog on Azure, then added security features over three days. I deleted the resources afterward to avoid charges, so I've included screenshots.

## What I did
- Deployed a PHP web app on Azure App Service using the free Azure domain
- Looked up the site's IP, DNS records, and location
- Created and bound a self-signed TLS certificate, and compared it to CA-signed and wildcard certificates
- Learned how Azure Key Vault stores keys, secrets, and certificates, and why access policies matter
- Compared Azure Front Door and Application Gateway, and learned what SSL offloading does
- Built a WAF custom rule that blocks traffic by country

## What I learned
A site can look finished and still have gaps. Certificates, access policies, and a WAF each close a different one, and none of them replaces the others.

[Read the full brief (PDF)](project-1-technical-brief.pdf)
