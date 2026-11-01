---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is done system-to-system via an API key, which is scoped to a specific property at a brand, so you must be sure you are sending the right key to act on data for an individual property.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kyc Hospitality Authentication
name_suffix: Authentication
oauth_flows: []
overview: KYC Hospitality declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: KYC Hospitality
provider_slug: kyc-hospitality
scheme_count: 1
schemes:
- evidence: 'API keys are opaque ASCII strings that you must send as a standard bearer header, as in:


    `Authorization: Bearer <key>`'
  header: Authorization
  how_to_obtain: API keys are issued by the KYC support team and will be sent to you via secure one-time-use channels.
  location: header
  name: API Key
  type: apiKey
slug: kyc-hospitality-authentication
source_filename: kyc-hospitality-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.kychospitality.com/authentication.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.kychospitality.com/authentication.md\nsources:\n- https://api-docs.kychospitality.com/authentication.md\n- https://api-docs.kychospitality.com/getting-started.md\ndescription: Authentication is done system-to-system via an API key, which is scoped to a specific property at a brand, so you must be sure you\n  are sending the right key to act on data for an individual property.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'API keys are opaque ASCII strings that you must send as a standard bearer header, as in:\n\n\n    `Authorization: Bearer <key>`'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are issued by the KYC support team and will be sent to you via secure one-time-use channels.\ndocs: https://api-docs.kychospitality.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/kyc-hospitality/authentication/kyc-hospitality-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hospitality
- Compliance
- IdentityVerification
- SaaS
---
