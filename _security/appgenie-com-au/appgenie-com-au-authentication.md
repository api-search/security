---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published by AppGenie
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: AppGenie Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppGenie declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AppGenie
provider_slug: appgenie-com-au
scheme_count: 3
schemes:
- evidence: Whether you’re using username/password authentication or public key authentication, FTP2SF handles the verification process seamlessly
  name: Username/Password
  type: other
- evidence: Whether you’re using username/password authentication or public key authentication, FTP2SF handles the verification process seamlessly
  name: Public Key
  type: other
- evidence: Authenticating SF CLI using a Json Web Token (JWT)
  flows:
  - jwt
  how_to_obtain: Create a Connected App in Salesforce, upload a digital certificate, and use the generated Consumer Key (client‑id) and the signed JWT file with the sf CLI command.
  name: JWT
  type: oauth2
slug: appgenie-com-au-authentication
source_filename: appgenie-com-au-authentication.yml
source_heading: Authentication Profile
source_url: https://appgenie.com.au/ftp2sf-sftp-auth
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://appgenie.com.au/ftp2sf-sftp-auth\nsources:\n- https://appgenie.com.au/ftp2sf-sftp-auth\n- https://appgenie.com.au/salesforce-jwt\ndescription: Authentication methods published by AppGenie\nschemes:\n- type: other\n  name: Username/Password\n  evidence: Whether you’re using username/password authentication or public key authentication, FTP2SF handles the verification process seamlessly\n- type: other\n  name: Public Key\n  evidence: Whether you’re using username/password authentication or public key authentication, FTP2SF handles the verification process seamlessly\n- type: oauth2\n  name: JWT\n  evidence: Authenticating SF CLI using a Json Web Token (JWT)\n  flows:\n  - jwt\n  how_to_obtain: Create a Connected App in Salesforce, upload a digital certificate, and use the generated Consumer Key (client‑id) and the signed\n    JWT file with the sf CLI command.\ndocs: https://appgenie.com.au/ftp2sf-sftp-auth\n"
source_yaml_url: https://artifacts.apis.io/appgenie-com-au/authentication/appgenie-com-au-authentication.yml
summary_line: 3 schemes
tags:
- B2B
- Cloud
- Salesforce
- DevSecOps
- Consulting
---
