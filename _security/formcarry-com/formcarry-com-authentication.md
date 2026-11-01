---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formcarry-com-api-openapi-generated.yml
  format: yaml
  label: formcarry-com api API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formcarry-com/openapi/_ae-authored/formcarry-com-api-openapi-generated.yml
- filename: formcarry-com-api-reference-openapi-generated.yml
  format: yaml
  label: formcarry-com api reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formcarry-com/openapi/_ae-authored/formcarry-com-api-reference-openapi-generated.yml
auth_types: []
description: 'Formcarry provides two authentication methods: a Bearer token for the current API and an api_key header for the legacy API.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Formcarry Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: formcarry-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: formcarry-com
provider_slug: formcarry-com
scheme_count: 2
schemes:
- evidence: Pass the key in the Authorization header on every request using the Bearer scheme.
  header: Authorization
  how_to_obtain: Generate an API key in the Formcarry dashboard under API Keys, choose scopes, and copy the key (prefixed with fc_live_).
  location: header
  name: Bearer token
  type: http-bearer
- evidence: The legacy API authenticates every request with an API key sent in the api_key header.
  header: api_key
  how_to_obtain: Open the Formcarry dashboard, go to Settings → API Keys, and copy your key.
  location: header
  name: Legacy API key
  type: apiKey
slug: formcarry-com-authentication
source_filename: formcarry-com-authentication.yml
source_heading: Authentication Profile
source_url: https://formcarry.com/docs/api/authentication
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://formcarry.com/docs/api/authentication\nsources:\n- https://formcarry.com/docs/api/authentication\n- https://formcarry.com/docs/api/legacy/authentication\n- https://formcarry.com/docs/quickstart\n- https://formcarry.com/docs/email/gmail-smtp-setup\ndescription: 'Formcarry provides two authentication methods: a Bearer token for the current API and an api_key header for the legacy API.'\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Pass the key in the Authorization header on every request using the Bearer scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Formcarry dashboard under API Keys, choose scopes, and copy the key (prefixed with fc_live_).\n- type: apiKey\n  name: Legacy API key\n  evidence: The legacy API authenticates every request with an API key sent in the api_key header.\n  location: header\n \
  \ header: api_key\n  how_to_obtain: Open the Formcarry dashboard, go to Settings → API Keys, and copy your key.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://formcarry.com/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/formcarry-com/authentication/formcarry-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Forms
- Backend-as-a-Service
- Webhooks
---
