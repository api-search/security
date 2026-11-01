---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Esker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Esker declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Esker
provider_slug: esker
scheme_count: 1
schemes:
- description: Authentication via username and password through SessionService.Login method, which creates a session context used by other services
  docs: https://doc.esker.com/eskerondemand/cv_ly/en/webservices/Content/References/API/SessionService_Login_meth.html
  flow: 1. Call GetBindings to get service URLs, 2. Call Login with username/password to create session, 3. Use session ID in subsequent requests
  name: Session-based authentication
  parameters:
  - in: body
    name: userName
    required: true
  - in: body
    name: password
    required: true
  type: username_password
slug: esker-authentication
source_filename: esker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://doc.esker.com/eskerondemand/cv_ly/en/webservices/Content/Quick_Start.html\nschemes:\n- type: username_password\n  name: Session-based authentication\n  description: \"Authentication via username and password through SessionService.Login method, which creates a session context used by other services\"\n  docs: https://doc.esker.com/eskerondemand/cv_ly/en/webservices/Content/References/API/SessionService_Login_meth.html\n  flow: \"1. Call GetBindings to get service URLs, 2. Call Login with username/password to create session, 3. Use session ID in subsequent requests\"\n  parameters:\n  - name: userName\n    in: body\n    required: true\n  - name: password\n    in: body\n    required: true"
source_yaml_url: https://artifacts.apis.io/esker/authentication/esker-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Accounts Payable
- Order-to-Cash
- Source-to-Pay
- Document Automation
- E-Invoicing
- Procurement
- SOAP
---
