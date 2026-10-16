---
anonymous_access: false
api_key_in: []
api_specs:
- filename: conveyor-openapi-generated.yml
  format: yaml
  label: Conveyor API
  slug: conveyor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conveyor/refs/heads/main/openapi/_ae-authored/conveyor-openapi-generated.yml
auth_types: []
description: Conveyor authentication methods as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Conveyor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conveyor declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Conveyor
provider_slug: conveyor
scheme_count: 2
schemes:
- evidence: This token authenticates to the Conveyor API. To successfully authenticate, you must include this token in the headers of your request.
  how_to_obtain: Generate an API token via the Conveyor UI under Settings → Integrations → Add Integration → Conveyor API.
  location: header
  name: Conveyor API Key
  type: apiKey
- evidence: To enable BYOAuth, your application will send Conveyor a **signed JSON Web Token (JWT)** containing the user’s information.
  how_to_obtain: Generate a signed JWT using a private key and include it as the `jwt` query parameter in the login URL.
  location: query
  name: Bring‑Your‑Own‑Auth JWT
  type: jwt
slug: conveyor-authentication
source_filename: conveyor-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.conveyor.com/docs/passwordless-authentication.md
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.conveyor.com/docs/passwordless-authentication.md\nsources:\n- https://docs.conveyor.com/docs/passwordless-authentication.md\n- https://docs.conveyor.com/docs/setting-up-the-salesforce-oauth-integration.md\n- https://docs.conveyor.com/docs/bring-your-own-auth.md\n- https://docs.conveyor.com/reference/api-token.md\ndescription: Conveyor authentication methods as documented\nschemes:\n- type: apiKey\n  name: Conveyor API Key\n  evidence: This token authenticates to the Conveyor API. To successfully authenticate, you must include this token in the headers of your request.\n  location: header\n  how_to_obtain: Generate an API token via the Conveyor UI under Settings → Integrations → Add Integration → Conveyor API.\n- type: jwt\n  name: Bring‑Your‑Own‑Auth JWT\n  evidence: To enable BYOAuth, your application will send Conveyor a **signed JSON Web Token (JWT)** containing\
  \ the user’s information.\n  location: query\n  how_to_obtain: Generate a signed JWT using a private key and include it as the `jwt` query parameter in the login URL.\nnote: No OAuth flows, passwordless passcode, or other authentication schemes provide sufficient details for header/query names or URLs, so they\n  are omitted.\ndocs: https://docs.conveyor.com/docs/passwordless-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conveyor/refs/heads/main/authentication/conveyor-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Security Questionnaire Automation
- RFP Automation
- Trust Center
- Customer Trust
- Compliance
- Knowledge Management
---
