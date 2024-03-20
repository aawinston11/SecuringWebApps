# Azure Security Features

## Part 1: Create a Front Door Instance

1. Log in to the Azure portal at https://portal.azure.com.
2. From the left menu, select "Networking."
3. Under "Inbound networking features," select "Azure Front Door."
4. On the next page, select "Create new" under "Front Door profile."
5. In the pane that opens on the right:
    - Name your Front Door "project1-FrontDoor."
    - Enter "AndreWebApp" for the Endpoint name.
    - The Endpoint hostname will be created automatically based on the Endpoint name.
    - Enter "RedTeam" for the Origin group name.
    - Select "Premium" for the Pricing Tier.
    - Click "OK" to close the pane.
6. Click "Create" to create the Front Door instance.
7. Verify that your Front Door instance has been set up correctly by selecting "Azure Front Door" again and ensuring that the message "Azure Front Door is configured for your web app" is displayed.

## Part 2: Analyze WAF Rule Sets

1. From the Azure portal, enter "web app" until "Web Application Firewall policies (WAF)" appears in the dropdown.
2. Select "Web Application Firewall policies (WAF)."
3. Choose your WAF policy (it will begin with "AndreWebAppfrontdoor").
4. Select "Managed rules" either from the left-hand toolbar or the box on the bottom of the page.
5. Scroll through the page to view the various rules.

## Part 3: Configure Custom WAF Rules

1. Select "Custom rules" from the toolbar on the left-hand side.
2. Click "+ Add custom rule."
3. In the pane that pops up:
    - Name your custom rule "Project1rule."
    - Leave the status and rule type at the default options.
    - Set the priority to 100.
    - Set the condition as follows:
      - Match type: Geo location
      - Match variable: Remoteaddr
      - Operation: is not
      - Select the three countries (USA, Canada, Australia)
      - Action: Deny traffic
4. Click "Add" to create the custom rule.

## Part 4: Analyze and Fix a Security Center Recommendation

1. Access Azure Security Center by selecting "Microsoft Defender for Cloud" from the toolbar on the left.
2. Review the recommendations provided by Azure Security Center, which continuously monitors the configuration of your app services for potential security vulnerabilities.
3. Select an individual recommendation to view the recommended steps to remediate it.
