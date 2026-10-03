---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formfeed-account-api-openapi.yml
  format: yaml
  label: Formfeed Account API
  slug: formfeed-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-account-api-openapi.yml
- filename: formfeed-brand-api-openapi.yml
  format: yaml
  label: Formfeed Brand API
  slug: formfeed-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-brand-api-openapi.yml
- filename: formfeed-compat-api-openapi.yml
  format: yaml
  label: Formfeed Compat API
  slug: formfeed-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-compat-api-openapi.yml
- filename: formfeed-files-api-openapi.yml
  format: yaml
  label: Formfeed Files API
  slug: formfeed-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-files-api-openapi.yml
- filename: formfeed-partials-api-openapi.yml
  format: yaml
  label: Formfeed Partials API
  slug: formfeed-partials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-partials-api-openapi.yml
- filename: formfeed-pdf-tools-api-openapi.yml
  format: yaml
  label: Formfeed PDF tools API
  slug: formfeed-pdf-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-pdf-tools-api-openapi.yml
- filename: formfeed-renders-api-openapi.yml
  format: yaml
  label: Formfeed Renders API
  slug: formfeed-renders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-renders-api-openapi.yml
- filename: formfeed-templates-api-openapi.yml
  format: yaml
  label: Formfeed Templates API
  slug: formfeed-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-templates-api-openapi.yml
- filename: formfeed-webhooks-api-openapi.yml
  format: yaml
  label: Formfeed Webhooks API
  slug: formfeed-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-webhooks-api-openapi.yml
auth_types: []
description: Formfeed API authentication uses API keys either as a Bearer token in the Authorization header or as an X‑API‑Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Formfeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formfeed declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Formfeed
provider_slug: formfeed
scheme_count: 2
schemes:
- evidence: 'Authorization : Bearer ff_live_3f9c...'
  header: Authorization
  how_to_obtain: Keys are created in the app under API keys, belong to exactly one workspace, and are shown once.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'X-API-Key: ff_live_3f9c... is accepted as well.'
  header: X-API-Key
  how_to_obtain: Keys are created in the app under API keys, belong to exactly one workspace, and are shown once.
  location: header
  name: X‑API‑Key header
  type: apiKey
slug: formfeed-authentication
source_filename: formfeed-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.formfeed.dev/getting-started/two-factor-authentication
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.formfeed.dev/getting-started/two-factor-authentication\nsources:\n- https://docs.formfeed.dev/getting-started/two-factor-authentication\n- https://docs.formfeed.dev/api/authentication\n- https://docs.formfeed.dev/de/api/authentication\n- https://docs.formfeed.dev/api/overview\ndescription: Formfeed API authentication uses API keys either as a Bearer token in the Authorization header or as an X‑API‑Key header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authorization : Bearer ff_live_3f9c...'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are created in the app under API keys, belong to exactly one workspace, and are shown once.\n- type: apiKey\n  name: X‑API‑Key header\n  evidence: 'X-API-Key: ff_live_3f9c... is accepted as well.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Keys are created in the app under\
  \ API keys, belong to exactly one workspace, and are shown once.\nnote: No OAuth2 flows are documented.\ndocs: https://docs.formfeed.dev/getting-started/two-factor-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/authentication/formfeed-authentication.yml
summary_line: 2 schemes
tags:
- PDF
- Image Generation
- Templates
- Developer Tools
- Software-as-a-Service
---
