---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Vishwa APIs uses an API key passed in the request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vishwa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vishwa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vishwa
provider_slug: vishwa
scheme_count: 1
schemes:
- evidence: '''XP-API-Key'' : "<token>" , # Replace <token> with your actual API key'
  header: XP-API-Key
  how_to_obtain: Obtain an API key from Vishwa and include it as the value of the XP-API-Key header in each request.
  location: header
  name: XP-API-Key
  type: apiKey
slug: vishwa-authentication
source_filename: vishwa-authentication.yml
source_heading: Authentication Profile
source_url: https://www.vishwa.ai/docs/quickstart/automate-invoice-processing
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.vishwa.ai/docs/quickstart/automate-invoice-processing\nsources:\n- https://www.vishwa.ai/docs/quickstart/automate-invoice-processing\n- https://www.vishwa.ai/docs/quickstart/convert-menu-to-excel\n- https://www.vishwa.ai/docs/quickstart/match-and-merge-docs\n- https://www.vishwa.ai/docs/quickstart/account-recon\ndescription: Authentication for Vishwa APIs uses an API key passed in the request header.\nschemes:\n- type: apiKey\n  name: XP-API-Key\n  evidence: '''XP-API-Key'' : \"<token>\" , # Replace <token> with your actual API key'\n  location: header\n  header: XP-API-Key\n  how_to_obtain: Obtain an API key from Vishwa and include it as the value of the XP-API-Key header in each request.\nnote: No OAuth2, HTTP Bearer, or other authentication schemes are documented on the provided pages.\ndocs: https://www.vishwa.ai/docs/quickstart/automate-invoice-processing\n"
source_yaml_url: https://artifacts.apis.io/vishwa/authentication/vishwa-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- FinTech
- Underwriting
- Credit
---
