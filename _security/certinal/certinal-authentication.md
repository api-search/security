---
anonymous_access: false
api_key_in: []
api_specs:
- filename: certinal-openapi-generated.yml
  format: yaml
  label: Certinal API
  slug: certinal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certinal/refs/heads/main/openapi/_ae-authored/certinal-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Certinal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Certinal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Certinal
provider_slug: certinal
scheme_count: 1
schemes:
- evidence: Certinal eSign supports the OAuth2 Client Credentials Grant to generate your access token with ease.
  flows:
  - client_credentials
  how_to_obtain: Log in to your Certinal eSign account, go to the More tab, click Create Custom Integration, and copy your Client ID, Secret, and API URL.
  name: OAuth2 Client Credentials
  token_url: https://esign-staging.certinal.com/auth/v1/token
  type: oauth2
slug: certinal-authentication
source_filename: certinal-authentication.yml
source_heading: Authentication Profile
source_url: https://certinal.stoplight.io/docs/api/b6b6c2d4906e9-authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://certinal.stoplight.io/docs/api/b6b6c2d4906e9-authentication\nsources:\n- https://certinal.stoplight.io/docs/api/b6b6c2d4906e9-authentication\n- https://certinal.stoplight.io/docs/api/q8v4vixymc0m7-o-auth-2-0-client-credentials-grant-flow-api\n- https://certinal.stoplight.io/docs/api/25t2fujer3i1u-remote-signing-with-email-or-sms-based-authentication\n- https://certinal.stoplight.io/docs/api/3fr7rwlmnk53b-in-person-signing-in-presence-of-a-staff\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Certinal eSign supports the OAuth2 Client Credentials Grant to generate your access token with ease.\n  flows:\n  - client_credentials\n  token_url: https://esign-staging.certinal.com/auth/v1/token\n  how_to_obtain: Log in to your Certinal eSign account, go to the More tab, click Create Custom Integration, and copy your Client ID, Secret,\n    and API URL.\n\
  docs: https://certinal.stoplight.io/docs/api/b6b6c2d4906e9-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certinal/refs/heads/main/authentication/certinal-authentication.yml
summary_line: 1 scheme
tags:
- Healthcare
- Consent
- Compliance
- eSignature
- EHR Integration
- Regulatory
---
