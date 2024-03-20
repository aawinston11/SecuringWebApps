# Securing Web App

## Part 1: Create a Key Vault

1. Log in to the Azure portal at https://portal.azure.com.
2. Navigate to "Key vaults" from the Azure search field.
3. Click on "+ Create" to create a new key vault.
4. Fill in the required information:
    - Subscription/Resource Group
    - Key Vault Name (must be globally unique)
    - Region
    - Pricing tier (choose "Standard")
5. Review the settings and click "Review + Create" to create the key vault.

## Part 2: Create a Self-Signed Certificate

1. Access the Cloud Shell from the Azure portal.
2. Use OpenSSL to generate a self-signed certificate
3. Answer the prompted questions about your certificate.
4. View the newly created key (.key) and certificate (.crt) using ls.
5. Convert the certificate and key to PFX format using Openssl
6. Enter a password to encrypt your PFX key.
7. Download the PFX certificate.

## Part 3: Import and Bind Your Self-Signed Certificate to Your Web App

1. Select "Key Vaults" from the Azure portal and choose your key vault.
2. Navigate to "Certificates" and click on "+ Generate/Import."
3. Choose "Import" as the method of certificate creation.
4. Upload the PFX certificate and enter the password.
5. Click "Create" to upload the certificate.
6. Return to your web application and select "TLS/SSL Settings."
7. Import the PFX certificate from the key vault.
8. Bind the certificate to your domain.

## Part 4: Create and Bind an App Service Managed Certificate

1. Return to "TLS/SSL settings" under your web application.
2. Select "Private Key Certificates" and click on "+ Create App Service Managed Certificates."
3. Choose your domain and click "Create."
4. Return to the "Bindings" tab and add a TLS/SSL binding.
5. Select your domain and the new certificate.
6. Add the binding.
7. Verify that there are no warnings displayed when accessing your website.
