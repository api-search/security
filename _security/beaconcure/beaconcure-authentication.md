---
api_key_in:
- undocumented
auth_types:
- apiKey
- ipAllowlist
description: ''
kind: authentication
layout: security
method: searched
name: Beaconcure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beaconcure secures its APIs with apiKey and ipAllowlist across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Beaconcure
provider_slug: beaconcure
scheme_count: 2
schemes:
- description: Beaconcure instructs prospective users to "log in with your test key and data, or use the API link you received from Beaconcure's customer success team." A per-customer key is therefore issued out of band by customer success; the transport location of that key is not documented publicly.
  in: undocumented
  name: verify-api-key
  parameter: undocumented
  sources:
  - https://beaconcure.com/api/
  type: apiKey
  x-evidence:
    fetched: '2026-08-06'
    http_status: 200
    url: https://beaconcure.com/api/
- description: 'The API endpoint itself is network-restricted: "The API link has restricted access to only the users on the IP whitelist provided by your organization during the onboarding process." Access is therefore gated at the network layer in addition to any credential.'
  name: ip-allowlist
  sources:
  - https://beaconcure.com/api/
  type: networkControl
  x-evidence:
    fetched: '2026-08-06'
    http_status: 200
    url: https://beaconcure.com/api/
slug: beaconcure-authentication
source_filename: beaconcure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://beaconcure.com/api/\ndocs: https://beaconcure.com/api/\napi: Beaconcure Verify API\nsummary:\n  types:\n  - apiKey\n  - ipAllowlist\n  api_key_in:\n  - undocumented\n  oauth2_flows: []\n  note: 'Beaconcure publishes no OpenAPI, no auth reference page and no public developer\n    portal. Everything recorded here is stated in prose on the single public Verify\n    API page; the concrete mechanics (header vs query parameter, key format, rotation,\n    token lifetime) are not published anywhere a member of the public can reach.'\nschemes:\n- name: verify-api-key\n  type: apiKey\n  in: undocumented\n  parameter: undocumented\n  description: 'Beaconcure instructs prospective users to \"log in with your test key\n    and data, or use the API link you received from Beaconcure''s customer success\n    team.\" A per-customer key is therefore issued out of band by customer success;\n    the transport location of that key is not\
  \ documented publicly.'\n  sources:\n  - https://beaconcure.com/api/\n  x-evidence:\n    fetched: '2026-08-06'\n    url: https://beaconcure.com/api/\n    http_status: 200\n- name: ip-allowlist\n  type: networkControl\n  description: 'The API endpoint itself is network-restricted: \"The API link has restricted\n    access to only the users on the IP whitelist provided by your organization during\n    the onboarding process.\" Access is therefore gated at the network layer in addition\n    to any credential.'\n  sources:\n  - https://beaconcure.com/api/\n  x-evidence:\n    fetched: '2026-08-06'\n    url: https://beaconcure.com/api/\n    http_status: 200\nissuance:\n  self_service: false\n  channel: Beaconcure customer success team\n  note: There is no public sign-up, no key-provisioning console and no sandbox a non-customer\n    can reach.\ndata_isolation:\n  description: 'Beaconcure states the API reads a partial clone of the customer''s\n    data rather than the live Verify application\
  \ — \"it doesn''t affect your live data\n    nor does it interact with Verify''s application\" — and that the API database is\n    \"encrypted with rotational keys.\"'\n  source: https://beaconcure.com/api/\ngaps:\n- No machine-readable security scheme (no OpenAPI, Swagger, or OIDC discovery document).\n- Key transport (header name / query parameter) is not published.\n- No documented token lifetime, rotation policy for customer keys, or revocation flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconcure/refs/heads/main/authentication/beaconcure-authentication.yml
summary_line: apiKey/ipAllowlist · 2 schemes
tags:
- Company
- Clinical Trials
- Clinical Data
- Life Sciences
- Pharmaceuticals
- Data Validation
- Quality Control
- Artificial Intelligence
- Biometrics
- Healthcare
---
