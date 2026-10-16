---
anonymous_access: false
api_key_in: []
api_specs:
- filename: helpjuice-openapi-generated.yml
  format: yaml
  label: Helpjuice API
  slug: helpjuice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpjuice/refs/heads/main/openapi/_ae-authored/helpjuice-openapi-generated.yml
auth_types: []
description: Authentication methods for Helpjuice as documented
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Helpjuice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helpjuice declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Helpjuice
provider_slug: helpjuice
scheme_count: 4
schemes:
- evidence: To interact with Helpjuice's API v3, you'll need a unique API key.
  name: Helpjuice API Key
  type: apiKey
- evidence: Helpjuice supports ADFS SSO, allowing organizations to integrate their Active Directory Federation Services for centralized authentication.
  name: ADFS SSO
  type: other
- evidence: Helpjuice allows users to sign in using their Google accounts, including accounts under custom company domains.
  name: Google Sign-In
  type: other
- evidence: 'redirect the user back to Helpjuice using the format: https://helpjuice.com/jwt/YOUR_SUBDOMAIN?jwt=YOUR_ENCODED_TOKEN'
  how_to_obtain: Generate a signed JWT using the shared key provided by Helpjuice and include it as the 'jwt' query parameter when redirecting back.
  location: query
  name: JWT SSO
  type: jwt
slug: helpjuice-authentication
source_filename: helpjuice-authentication.yml
source_heading: Authentication Profile
source_url: https://help.helpjuice.com/en_US/api-v3-webhooks/284079-how-do-i-get-my-api-key
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.helpjuice.com/en_US/api-v3-webhooks/284079-how-do-i-get-my-api-key\nsources:\n- https://help.helpjuice.com/en_US/api-v3-webhooks/284079-how-do-i-get-my-api-key\n- https://help.helpjuice.com/en_US/authentication/adfs-sso\n- https://help.helpjuice.com/en_US/authentication/google-sign-in\n- https://help.helpjuice.com/en_US/authentication/sso-with-json-web-token\ndescription: Authentication methods for Helpjuice as documented\nschemes:\n- type: apiKey\n  name: Helpjuice API Key\n  evidence: To interact with Helpjuice's API v3, you'll need a unique API key.\n- type: other\n  name: ADFS SSO\n  evidence: Helpjuice supports ADFS SSO, allowing organizations to integrate their Active Directory Federation Services for centralized authentication.\n- type: other\n  name: Google Sign-In\n  evidence: Helpjuice allows users to sign in using their Google accounts, including accounts\
  \ under custom company domains.\n- type: jwt\n  name: JWT SSO\n  evidence: 'redirect the user back to Helpjuice using the format: https://helpjuice.com/jwt/YOUR_SUBDOMAIN?jwt=YOUR_ENCODED_TOKEN'\n  location: query\n  how_to_obtain: Generate a signed JWT using the shared key provided by Helpjuice and include it as the 'jwt' query parameter when redirecting\n    back.\ndocs: https://help.helpjuice.com/en_US/api-v3-webhooks/284079-how-do-i-get-my-api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpjuice/refs/heads/main/authentication/helpjuice-authentication.yml
summary_line: 4 schemes
tags:
- Knowledge Base
- SaaS
- Customer Support
- AI
- Documentation
---
