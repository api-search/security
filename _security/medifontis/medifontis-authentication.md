---
anonymous_access: false
api_key_in: []
auth_types: []
description: Medifontis authenticates requests using an API key that can be sent either as a Bearer token in the Authorization header or as a plain API key in the X‑Api‑Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Medifontis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medifontis declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Medifontis
provider_slug: medifontis
scheme_count: 2
schemes:
- evidence: Send the key in the Authorization header with the Bearer scheme, or in the X-Api-Key header.
  header: Authorization
  how_to_obtain: Create a key on the signup page; the key starts with mf_live_ and is shown only once.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Send the key in the Authorization header with the Bearer scheme, or in the X-Api-Key header.
  header: X-Api-Key
  how_to_obtain: Create a key on the signup page; the key starts with mf_live_ and is shown only once.
  location: header
  name: X‑Api‑Key header
  type: apiKey
slug: medifontis-authentication
source_filename: medifontis-authentication.yml
source_heading: Authentication Profile
source_url: https://www.medifontis.com/us/en/docs/authentication/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.medifontis.com/us/en/docs/authentication/\nsources:\n- https://www.medifontis.com/us/en/docs/authentication/\n- https://www.medifontis.com/us/en/docs/authentication/\n- https://www.medifontis.com/us/en/signup/\n- https://www.medifontis.com/us/en/docs/quickstart/\ndescription: Medifontis authenticates requests using an API key that can be sent either as a Bearer token in the Authorization header or as a\n  plain API key in the X‑Api‑Key header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Send the key in the Authorization header with the Bearer scheme, or in the X-Api-Key header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key on the signup page; the key starts with mf_live_ and is shown only once.\n- type: apiKey\n  name: X‑Api‑Key header\n  evidence: Send the key in the Authorization header with the Bearer scheme, or\
  \ in the X-Api-Key header.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create a key on the signup page; the key starts with mf_live_ and is shown only once.\nnote: No OAuth2, http‑basic, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://www.medifontis.com/us/en/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/medifontis/authentication/medifontis-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- API
- FDA
- Drugs
---
