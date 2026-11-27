---
anonymous_access: false
api_key_in: []
api_specs:
- filename: awell-openapi-generated.yml
  format: yaml
  label: Awell API
  slug: awell-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awell/openapi/_ae-authored/awell-openapi-generated.yml
auth_types: []
description: Authentication methods for Awell APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Awell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Awell declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Awell
provider_slug: awell
scheme_count: 2
schemes:
- evidence: Put the key in an `apiKey` header on every request.
  header: apiKey
  how_to_obtain: An administrator creates API keys in the CareOps portal – open Integrations → API keys tab → Create API key.
  location: header
  name: apiKey
  type: apiKey
- evidence: Add a second API call action for the real request, and pass the stored token in the Authorization header as a variable.
  header: Authorization
  how_to_obtain: Obtain a client ID and client secret from the target system’s administrator or documentation, then POST them to the system’s token endpoint using the client credentials grant.
  location: header
  name: client_credentials
  type: oauth2
slug: awell-authentication
source_filename: awell-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.awellhealth.com/docs/connect-systems/oauth-client-credentials.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.awellhealth.com/docs/connect-systems/oauth-client-credentials.md\nsources:\n- https://docs.awellhealth.com/docs/connect-systems/oauth-client-credentials.md\n- https://docs.awellhealth.com/api-reference/guides/authentication.md\n- https://docs.awellhealth.com/changelog#2023-06-01-api-keys-and-new-condition-operators\n- https://docs.awellhealth.com/docs/connect-systems/oauth-client-credentials\ndescription: Authentication methods for Awell APIs\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Put the key in an `apiKey` header on every request.\n  location: header\n  header: apiKey\n  how_to_obtain: An administrator creates API keys in the CareOps portal – open Integrations → API keys tab → Create API key.\n- type: oauth2\n  name: client_credentials\n  evidence: Add a second API call action for the real request, and pass the stored token in the Authorization header\
  \ as a variable.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a client ID and client secret from the target system’s administrator or documentation, then POST them to the system’s\n    token endpoint using the client credentials grant.\ndocs: https://docs.awellhealth.com/docs/connect-systems/oauth-client-credentials.md\n"
source_yaml_url: https://artifacts.apis.io/awell/authentication/awell-authentication.yml
summary_line: 2 schemes
tags:
- Healthcare
- Artificial Intelligence
- CareOps
- Platform
- Integration
---
