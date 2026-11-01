---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes as documented
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Syvizo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syvizo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Syvizo
provider_slug: syvizo
scheme_count: 1
schemes:
- evidence: This value is typically sent in Authorization HTTP header to the backend API
  header: Authorization
  location: header
  name: Basic Auth
  type: http-basic
slug: syvizo-authentication
source_filename: syvizo-authentication.yml
source_heading: Authentication Profile
source_url: https://syvizo.com.au/docs/Manage_API_Flows/Security/Basic_Auth.html
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://syvizo.com.au/docs/Manage_API_Flows/Security/Basic_Auth.html\nsources:\n- https://syvizo.com.au/docs/Manage_API_Flows/Security/Basic_Auth.html\n- https://syvizo.com.au/docs/Manage_API_Flows/Security/Decode_Auth.html\n- https://syvizo.com.au/docs/Manage_API_Flows/Security/Generate_JWT_Token.html\n- https://syvizo.com.au/docs/Manage_API_Flows/Security/Verify_JWT_Token.html\ndescription: Authentication schemes as documented\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: This value is typically sent in Authorization HTTP header to the backend API\n  location: header\n  header: Authorization\ndocs: https://syvizo.com.au/docs/Manage_API_Flows/Security/Basic_Auth.html\n"
source_yaml_url: https://artifacts.apis.io/syvizo/authentication/syvizo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API Platform
- Low-Code
- No-Code
- Integration
---
