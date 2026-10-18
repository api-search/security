---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes published for Eagle Eye
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Eagle Eye Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eagle Eye declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Eagle Eye
provider_slug: eagle-eye
scheme_count: 2
schemes:
- evidence: To maintain a secure API and protect the data held within the platform all of Eagle Eye API's are secured with a ClientId and Hash passed in the headers of every request.
  header: X-EES-AUTH-CLIENT-ID
  how_to_obtain: Contact your Account Manager to have the ClientId set up during onboarding.
  location: header
  name: X-EES-AUTH-CLIENT-ID
  type: apiKey
- evidence: To maintain a secure API and protect the data held within the platform all of Eagle Eye API's are secured with a ClientId and Hash passed in the headers of every request.
  header: X-EES-AUTH-HASH
  how_to_obtain: Generate the hash for each request by concatenating uri + body + secret and hashing with SHA256 as described in the documentation.
  location: header
  name: X-EES-AUTH-HASH
  type: apiKey
slug: eagle-eye-authentication
source_filename: eagle-eye-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.eagleeye.com/eagleeye-developer/docs/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.eagleeye.com/eagleeye-developer/docs/authentication.md\nsources:\n- https://developer.eagleeye.com/eagleeye-developer/docs/authentication.md\n- https://developer.eagleeye.com/eagleeye-developer/docs/api-authentication.md\n- https://developer.eagleeye.com/eagleeye-developer/docs/air-dashboard-authentication.md\n- https://developer.eagleeye.com/eagleeye-developer/docs/authentication\ndescription: Authentication schemes published for Eagle Eye\nschemes:\n- type: apiKey\n  name: X-EES-AUTH-CLIENT-ID\n  evidence: To maintain a secure API and protect the data held within the platform all of Eagle Eye API's are secured with a ClientId and Hash\n    passed in the headers of every request.\n  location: header\n  header: X-EES-AUTH-CLIENT-ID\n  how_to_obtain: Contact your Account Manager to have the ClientId set up during onboarding.\n- type: apiKey\n  name: X-EES-AUTH-HASH\n\
  \  evidence: To maintain a secure API and protect the data held within the platform all of Eagle Eye API's are secured with a ClientId and Hash\n    passed in the headers of every request.\n  location: header\n  header: X-EES-AUTH-HASH\n  how_to_obtain: Generate the hash for each request by concatenating uri + body + secret and hashing with SHA256 as described in the documentation.\nnote: Dashboard authentication methods (2FA, SAML) are user‑interface flows and not applicable to API authentication.\ndocs: https://developer.eagleeye.com/eagleeye-developer/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eagle-eye/refs/heads/main/authentication/eagle-eye-authentication.yml
summary_line: 2 schemes
tags:
- Loyalty
- Personalization
- Promotions
- Retail
- Artificial Intelligence
- Omnichannel
- Gift Cards
---
