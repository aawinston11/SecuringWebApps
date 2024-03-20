# Building a Secure Web Application with GoDaddy Domain

Today, I embarked on the journey of building, hosting, and designing your own web application, 
fortified with security measures, and mapped to a custom domain obtained from GoDaddy. Below are 
the detailed steps I followed to achieve this:

## Getting Started / Prerequisites
Before diving into building your web application, you ensured the following prerequisites were met:

- Created your own Azure Account and subscription.
- Established a resource group (e.g., RedTeam) within Azure.

## Part 1: Create an Azure Web App
1. Access Azure Portal: Logged in to the Azure portal (https://portal.azure.com).
2. Navigate to App Services: Selected "App Services" from the Azure search field.
3. Create Web Application: Clicked on "+ Create" to initiate the creation process.
4. Configure Basics:
    - Selected appropriate subscription and resource group.
    - Named the instance (e.g., "Bobssecurityresume").
    - Chose "Code" for publishing and "PHP 8.0" as the runtime stack.
    - Selected "Linux" as the operating system.
    - Chose the same region used previously.
5. Configure App Service Plan:
    - Created a new pricing plan named "project1plan".
    - Selected "Basic B1" pricing tier.
6. Review and Create: Confirmed selections and clicked "Create" to create the web app.

## Part 2a: Choose a Domain with GoDaddy
1. Navigate to GoDaddy: Accessed GoDaddy's website.
2. Select Domain: Picked a unique domain name for the cyber-blog.
3. Complete Purchase: Followed the checkout process, ensuring the domain was available and selecting the desired duration.
4. Create GoDaddy Account: Created or logged into GoDaddy account.
5. Complete Payment: Finalized the purchase.

## Part 2b: Map Your Custom Domain to Azure’s App Service
1. Custom Domain Configuration:
    - Navigated back to Azure App Service and selected "Custom domains."
    - Added the custom domain obtained from GoDaddy and validated it.
    - Updated DNS records in GoDaddy to point to Azure's app service.

## Part 3: Deploy a Container on the Web App
1. Deploy Docker Container:
    - Used Azure Cloud Shell to deploy a Docker container containing the cyber-blog framework.
    - Configured the web app with the provided container image.
    - Verified successful deployment by checking the unique domain.

## Part 4: Design Your Custom Web Application
1. Customize Webpage:
    - Accessed HTML files of the web application via SSH.
    - Edited HTML files to customize various elements of the webpage:
      - Personal information (name, email, LinkedIn profile link).
      - Introduction.
      - Picture.
      - Two custom blog posts on cybersecurity topics.
2. Backup HTML Files: Ensured to back up HTML files after each update to prevent loss of changes.
