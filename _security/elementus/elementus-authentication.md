---
api_key_in: []
auth_types: []
description: 'Elementus publishes no authentication documentation page that is reachable — every docs host is down (see well-known/elementus-well-known.yml). This profile is derived from Elementus'' own first-party public API example client, which is the only live public description of how the Attribution API is called. It is a faithful reading of that source, not a reading of a spec: there is no OpenAPI to derive securitySchemes from.'
kind: authentication
layout: security
method: derived
name: Elementus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elementus declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Elementus
provider_slug: elementus
scheme_count: 1
schemes:
- applies_to: all documented operations
  description: 'A per-account API key sent on every request in the X-API-Key header. The example client reads it from an ELEMENTUS_API_KEY environment variable and sets it once on the session, alongside Content-Type: application/json.'
  evidence: 'ElementusClient.__init__ sets self.headers = {"X-API-Key": api_key, "Content-Type": "application/json"} and applies it to every request.'
  id: apiKey
  in: header
  name: X-API-Key
  type: apiKey
slug: elementus-authentication
source_filename: elementus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: https://raw.githubusercontent.com/elementus-io/api-example/master/elementus.py\nname: Elementus Attribution API authentication\napi: Elementus Attribution API\nbase_url: https://attribution-api.elementus.io\ndescription: >-\n  Elementus publishes no authentication documentation page that is reachable —\n  every docs host is down (see well-known/elementus-well-known.yml). This\n  profile is derived from Elementus' own first-party public API example client,\n  which is the only live public description of how the Attribution API is\n  called. It is a faithful reading of that source, not a reading of a spec:\n  there is no OpenAPI to derive securitySchemes from.\n\nderived_from:\n  repository: https://github.com/elementus-io/api-example\n  owner: elementus-io\n  first_party: true\n  file: elementus.py\n  last_commit: '2025-03-05'\n\nschemes:\n- id: apiKey\n  type: apiKey\n  in: header\n  name: X-API-Key\n  description: >-\n    A\
  \ per-account API key sent on every request in the X-API-Key header. The\n    example client reads it from an ELEMENTUS_API_KEY environment variable and\n    sets it once on the session, alongside Content-Type: application/json.\n  evidence: >-\n    ElementusClient.__init__ sets self.headers = {\"X-API-Key\": api_key,\n    \"Content-Type\": \"application/json\"} and applies it to every request.\n  applies_to: all documented operations\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: none-published\nrotation_policy: not-published\nkey_issuance: not-published\n\nnotes:\n- No OAuth2, OpenID Connect or mTLS surface was found on any Elementus host or\n  in any first-party source.\n- Because the scheme is a flat API key with no scope surface, no scopes/\n  artifact was written — an empty scope catalog would assert a permission model\n  the provider does not have.\n- Key issuance is presumably a sales/onboarding motion; no self-serve signup\n  page could be reached to confirm\
  \ it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elementus/refs/heads/main/authentication/elementus-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Blockchain
- Cryptocurrency
- Analytics
- Compliance
- Financial Crime
- Sanctions Screening
- Data
- Web3
---
