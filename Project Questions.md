# Project Questions

## Cloud Security Questions
- Azure Web Application Gateway vs. Azure Front Door: Both provide load balancing, but the former is regional while the latter is global.
- SSL Offloading: Removing SSL-based encryption to enhance server performance.
- WAF OSI Layer: WAF operates at Layer 7 of the OSI model.
- WAF Managed Rule Example - Directory Traversal: Exploits insufficient security validation of file names to access files outside the web root folder.
- Impact of WAF Custom Rule Blocking Canadian Traffic: It could potentially block Canadian visitors, but there are ways around location-based blocks.

## Cloud Questions
- Cloud Tenant: A cloud tenant refers to an individual or organization that rents or subscribes to cloud resources or services.
- Key Vault Access Policy: Access policies are crucial for security, ensuring the principle of least privilege, auditability, and data protection.
- Key Vault Components:
    - Keys: Used for encryption and decryption.
    - Secrets: Confidential information used for authentication.
    - Certificates: Establish identity for secure communication.
 
## Cryptography Questions
- Advantages of Self-Signed Certificates: They are cost-effective, provide full control, and can be quickly generated and deployed.
- Disadvantages of Self-Signed Certificates: Lack of inherent trust, administrative overhead, and potential compatibility issues.
- Wildcard Certificate: A wildcard certificate can be used with multiple subdomains of a domain.
- Reason for SSL 3.0 Exclusion: SSL 3.0 is obsolete and vulnerable to cryptography attacks.

## Networking Questions

- Domain Selection: I opted for a GoDaddy domain, which was pulled from Cloudflare.
- Domain Name: andrewinston.com
- IP Address: 20.119.16.29
- Location: Ashburn, Virginia, USA
- NS Record:
  - nslookup andrewinston.com
  - Server:  UnKnown
  - Address:  192.168.40.9

  - Non-authoritative answer:
  - Name:    andrewinston.com
  - Address:  20.119.16.29

## Web Development Questions
- Runtime Stack: I selected a back-end runtime stack for my web application.
- Assets Directory: The /var/www/html/assets directory contains CSS files and images, primarily for front-end development purposes.
