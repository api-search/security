---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ciq-agent-api-openapi.yml
  format: yaml
  label: CIQ Agent API
  slug: ciq-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-agent-api-openapi.yml
- filename: ciq-ciq-api-api-openapi.yml
  format: yaml
  label: CIQ CIQ API
  slug: ciq-ciq-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-ciq-api-api-openapi.yml
- filename: ciq-data-api-openapi.yml
  format: yaml
  label: CIQ Data API
  slug: ciq-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-data-api-openapi.yml
- filename: ciq-dlv2-api-openapi.yml
  format: yaml
  label: CIQ Dlv2 API
  slug: ciq-dlv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-dlv2-api-openapi.yml
- filename: ciq-models-api-openapi.yml
  format: yaml
  label: CIQ Models API
  slug: ciq-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-models-api-openapi.yml
- filename: ciq-path-api-openapi.yml
  format: yaml
  label: CIQ Path API
  slug: ciq-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-path-api-openapi.yml
- filename: ciq-sources-api-openapi.yml
  format: yaml
  label: CIQ Sources API
  slug: ciq-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/openapi/ciq-sources-api-openapi.yml
auth_types: []
description: Authentication methods documented for CIQ products
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ciq Authentication
name_suffix: Authentication
oauth_flows: []
overview: CIQ declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CIQ
provider_slug: ciq
scheme_count: 2
schemes:
- evidence: With SAML configured, ELM acts as a Service Provider and delegates authentication to your identity provider (IdP).
  name: SAML 2.0
  type: other
- evidence: 'Authenticate API requests with a session or HTTP Basic auth: API .'
  header: Authorization
  location: header
  name: HTTP Basic
  type: http-basic
slug: ciq-authentication
source_filename: ciq-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ciq.com/ascender-pro/admin-guides/saml
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ciq.com/ascender-pro/admin-guides/saml\nsources:\n- https://docs.ciq.com/ascender-pro/admin-guides/saml\n- https://docs.ciq.com/elm/admin-guides/authentication\n- https://docs.ciq.com/fuzzball/appendices/web-ui-tunnel/visit-site\n- https://docs.ciq.com/fuzzball/sdk/sdk-auth\ndescription: Authentication methods documented for CIQ products\nschemes:\n- type: other\n  name: SAML 2.0\n  evidence: With SAML configured, ELM acts as a Service Provider and delegates authentication to your identity provider (IdP).\n- type: http-basic\n  name: HTTP Basic\n  evidence: 'Authenticate API requests with a session or HTTP Basic auth: API .'\n  location: header\n  header: Authorization\ndocs: https://docs.ciq.com/ascender-pro/admin-guides/saml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciq/refs/heads/main/authentication/ciq-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Infrastructure
- Open Source
- Enterprise
- Cloud
---
