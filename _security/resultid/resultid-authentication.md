---
api_key_in:
- header
api_specs:
- filename: resultid-api-openapi.yml
  format: yaml
  label: Resultid API
  slug: resultid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/openapi/resultid-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Resultid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Resultid secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Resultid
provider_slug: resultid
scheme_count: 1
schemes:
- encoded_as: request-header-parameter
  evidence: 'Every operation on https://docs.resultid.com/22_api_spec_test/ renders an Input parameters table whose single row is "X-API-Key | header | string | Nullable: No".'
  in: header
  name: XApiKeyHeader
  parameter: X-API-Key
  required: true
  sources:
  - openapi/resultid-api-openapi.yml
  type: apiKey
slug: resultid-authentication
source_filename: resultid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: https://docs.resultid.com/22_api_spec_test/\ndocs: https://docs.resultid.com/1_getting_started/\nnote: >-\n  Resultid's published schema does not declare an OpenAPI securityScheme - the API key\n  is rendered as a required X-API-Key request header parameter on every one of the nine\n  operations, which is how FastAPI emits a Header(...) dependency. derive-authentication.py\n  therefore found nothing to aggregate; this profile is transcribed by hand from the\n  provider's own rendered parameter tables and from the Getting Started page, which says\n  only \"Make requests using the API Key to the given endpoints\". Resultid does not publish\n  how a key is issued, rotated or scoped, and there is no OAuth, OIDC or mTLS surface.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  applies_to: all\n  operations_covered: 9\n  operations_total: 9\nschemes:\n- name: XApiKeyHeader\n  type: apiKey\n  in: header\n\
  \  parameter: X-API-Key\n  required: true\n  sources: [openapi/resultid-api-openapi.yml]\n  encoded_as: request-header-parameter\n  evidence: >-\n    Every operation on https://docs.resultid.com/22_api_spec_test/ renders an Input\n    parameters table whose single row is \"X-API-Key | header | string | Nullable: No\".\ngaps:\n- No key-issuance, rotation or revocation process is documented.\n- No scopes, permissions or per-key entitlement model is documented.\n- No securityScheme is declared in the schema, so the key requirement is only discoverable\n  per-operation rather than as an API-level security requirement.\n- No API base URL is published, so a key holder cannot determine where to send the header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/authentication/resultid-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Operational Intelligence
- Analytics
- Enterprise Software
- Artificial Intelligence
- Customer Experience
- Data Integration
- Revenue Intelligence
---
