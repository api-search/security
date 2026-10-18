---
anonymous_access: false
api_key_in: []
api_specs:
- filename: edgrapi-activist-api-openapi.yml
  format: yaml
  label: Paper and Beyond Activist API
  slug: edgrapi-activist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-activist-api-openapi.yml
- filename: edgrapi-events-api-openapi.yml
  format: yaml
  label: Paper and Beyond Events API
  slug: edgrapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-events-api-openapi.yml
- filename: edgrapi-filings-api-openapi.yml
  format: yaml
  label: Paper and Beyond Filings API
  slug: edgrapi-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-filings-api-openapi.yml
- filename: edgrapi-fundamentals-api-openapi.yml
  format: yaml
  label: Paper and Beyond Fundamentals API
  slug: edgrapi-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-fundamentals-api-openapi.yml
- filename: edgrapi-government-api-openapi.yml
  format: yaml
  label: Paper and Beyond Government API
  slug: edgrapi-government-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-government-api-openapi.yml
- filename: edgrapi-holdings-api-openapi.yml
  format: yaml
  label: Paper and Beyond Holdings API
  slug: edgrapi-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-holdings-api-openapi.yml
- filename: edgrapi-insider-api-openapi.yml
  format: yaml
  label: Paper and Beyond Insider API
  slug: edgrapi-insider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-insider-api-openapi.yml
- filename: edgrapi-meta-api-openapi.yml
  format: yaml
  label: Paper and Beyond Meta API
  slug: edgrapi-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-meta-api-openapi.yml
- filename: edgrapi-reference-api-openapi.yml
  format: yaml
  label: Paper and Beyond Reference API
  slug: edgrapi-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-reference-api-openapi.yml
- filename: edgrapi-search-api-openapi.yml
  format: yaml
  label: Paper and Beyond Search API
  slug: edgrapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-search-api-openapi.yml
- filename: edgrapi-webhooks-api-openapi.yml
  format: yaml
  label: Paper and Beyond Webhooks API
  slug: edgrapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-webhooks-api-openapi.yml
- filename: edgrapi-xbrl-api-openapi.yml
  format: yaml
  label: Paper and Beyond Xbrl API
  slug: edgrapi-xbrl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-xbrl-api-openapi.yml
auth_types: []
description: Authentication methods for Edgrapi as documented on the provider pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Edgrapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paper and Beyond declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Paper and Beyond
provider_slug: edgrapi
scheme_count: 2
schemes:
- evidence: 'Send your key on every request in the X-API-Key header:'
  header: X-API-Key
  how_to_obtain: Create and revoke keys in your dashboard; a key is minted on signup.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Use X-API-Key or Authorization: Bearer .'
  header: Authorization
  how_to_obtain: Use the same API key value prefixed with edgr_ as a bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: edgrapi-authentication
source_filename: edgrapi-authentication.yml
source_heading: Authentication Profile
source_url: https://edgrapi.com/docs/authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://edgrapi.com/docs/authentication\nsources:\n- https://edgrapi.com/docs/authentication\n- https://edgrapi.com/docs\ndescription: Authentication methods for Edgrapi as documented on the provider pages.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send your key on every request in the X-API-Key header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create and revoke keys in your dashboard; a key is minted on signup.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Use X-API-Key or Authorization: Bearer .'\n  location: header\n  header: Authorization\n  how_to_obtain: Use the same API key value prefixed with edgr_ as a bearer token.\nnote: No OAuth2, JWT, HMAC, MTLS, or other schemes are described on the pages.\ndocs: https://edgrapi.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/authentication/edgrapi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- Government
- Artificial Intelligence
---
