---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for RevOps webhooks uses an HMAC signature sent in a custom HTTP header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Revops Authentication
name_suffix: Authentication
oauth_flows: []
overview: RevOps declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RevOps
provider_slug: revops
scheme_count: 1
schemes:
- evidence: 'RevOps generates an HMAC signature of the request''s body contents and includes this information as a custom header:'
  header: X-RevOps-Content-Hmac
  how_to_obtain: The HMAC signature is generated using the webhook's verification key, which can be found at /integrations/webhooks/setup.
  location: header
  name: X-RevOps-Content-Hmac
  type: hmac
slug: revops-authentication
source_filename: revops-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.revops.io/webhooks/authentication/
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.revops.io/webhooks/authentication/\nsources:\n- https://docs.revops.io/webhooks/authentication/\n- https://docs.revops.io/signing-agreements/\n- https://docs.revops.io/signing-agreements/counter-signing-revops-deals/\n- https://docs.revops.io/signing-agreements/customer-notifications/\ndescription: Authentication for RevOps webhooks uses an HMAC signature sent in a custom HTTP header.\nschemes:\n- type: hmac\n  name: X-RevOps-Content-Hmac\n  evidence: 'RevOps generates an HMAC signature of the request''s body contents and includes this information as a custom header:'\n  location: header\n  header: X-RevOps-Content-Hmac\n  how_to_obtain: The HMAC signature is generated using the webhook's verification key, which can be found at /integrations/webhooks/setup.\nnote: No other authentication schemes (e.g., OAuth2, API keys, etc.) are documented on the provided pages.\n\
  docs: https://docs.revops.io/webhooks/authentication/\n"
source_yaml_url: https://artifacts.apis.io/revops/authentication/revops-authentication.yml
summary_line: 1 scheme
tags:
- CPQ
- Revenue-Operations
- SaaS
- Integrations
- Deal-Desk
---
