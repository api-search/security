---
anonymous_access: false
api_key_in: []
api_specs:
- filename: versori-platform-openapi.yml
  format: yaml
  label: Versori Platform API
  slug: versori-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/versori/openapi/versori-platform-openapi.yml
auth_types: []
description: Authentication methods supported by Versori as documented.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Versori Authentication
name_suffix: Authentication
oauth_flows: []
overview: Versori declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Versori
provider_slug: versori
scheme_count: 4
schemes:
- evidence: OAuth 2.0 is a standard authentication method for web applications, and is the one most recommended to use where the system being integrated supports it.
  flows:
  - authorization_code
  - client_credentials
  - password
  - refresh_token
  name: OAuth 2.0
  type: oauth2
- evidence: API Key is a standard authentication method for API applications. Versori supports arbitrary API keys which can be set in the header, query string or cookie.
  name: API Key
  type: apiKey
- evidence: 'HTTP Authorization is a standard authentication method for HTTP applications where the credential is set in the "Authorization" header. Versori supports the following authorization schemes: * Bearer'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: This creates an authentication method called "No Auth" with the type set to "None - Authentication Bypassed".
  name: No Auth
  type: other
slug: versori-authentication
source_filename: versori-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.versori.com/latest/how-it-works/connect.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.versori.com/latest/how-it-works/connect.md\nsources:\n- https://docs.versori.com/latest/how-it-works/connect.md\n- https://docs.versori.com/latest/guides/getting-started/connect/bypass-auth.md\n- https://docs.versori.com/latest/guides/auth-methods/introduction.md\n- https://docs.versori.com/latest/guides/auth-methods/api-key.md\ndescription: Authentication methods supported by Versori as documented.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth 2.0 is a standard authentication method for web applications, and is the one most recommended to use where the system being\n    integrated supports it.\n  flows:\n  - authorization_code\n  - client_credentials\n  - password\n  - refresh_token\n- type: apiKey\n  name: API Key\n  evidence: API Key is a standard authentication method for API applications. Versori supports arbitrary API keys which can be set in\
  \ the header,\n    query string or cookie.\n- type: http-bearer\n  name: Bearer\n  evidence: 'HTTP Authorization is a standard authentication method for HTTP applications where the credential is set in the \"Authorization\" header.\n    Versori supports the following authorization schemes: * Bearer'\n  location: header\n  header: Authorization\n- type: other\n  name: No Auth\n  evidence: This creates an authentication method called \"No Auth\" with the type set to \"None - Authentication Bypassed\".\ndocs: https://docs.versori.com/latest/how-it-works/connect.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/versori/authentication/versori-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Integration
- Artificial Intelligence
- Automation
- Platform
---
