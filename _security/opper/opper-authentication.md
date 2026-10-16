---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opper-account-api-openapi.yml
  format: yaml
  label: Opper AI Account API
  slug: opper-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-account-api-openapi.yml
- filename: opper-artifacts-api-openapi.yml
  format: yaml
  label: Opper AI Artifacts API
  slug: opper-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-artifacts-api-openapi.yml
- filename: opper-audio-api-openapi.yml
  format: yaml
  label: Opper AI Audio API
  slug: opper-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-audio-api-openapi.yml
- filename: opper-compatibility-api-openapi.yml
  format: yaml
  label: Opper AI Compatibility API
  slug: opper-compatibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-compatibility-api-openapi.yml
- filename: opper-files-api-openapi.yml
  format: yaml
  label: Opper AI Files API
  slug: opper-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-files-api-openapi.yml
- filename: opper-functions-api-openapi.yml
  format: yaml
  label: Opper AI Functions API
  slug: opper-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-functions-api-openapi.yml
- filename: opper-generations-api-openapi.yml
  format: yaml
  label: Opper AI Generations API
  slug: opper-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-generations-api-openapi.yml
- filename: opper-images-api-openapi.yml
  format: yaml
  label: Opper AI Images API
  slug: opper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-images-api-openapi.yml
- filename: opper-management-api-openapi.yml
  format: yaml
  label: Opper AI Management API
  slug: opper-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-management-api-openapi.yml
- filename: opper-models-api-openapi.yml
  format: yaml
  label: Opper AI Models API
  slug: opper-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-models-api-openapi.yml
- filename: opper-ocr-api-openapi.yml
  format: yaml
  label: Opper AI OCR API
  slug: opper-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-ocr-api-openapi.yml
- filename: opper-rerank-api-openapi.yml
  format: yaml
  label: Opper AI Rerank API
  slug: opper-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-rerank-api-openapi.yml
- filename: opper-roundtable-api-openapi.yml
  format: yaml
  label: Opper AI Roundtable API
  slug: opper-roundtable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-roundtable-api-openapi.yml
- filename: opper-spans-api-openapi.yml
  format: yaml
  label: Opper AI Spans API
  slug: opper-spans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-spans-api-openapi.yml
- filename: opper-system-api-openapi.yml
  format: yaml
  label: Opper AI System API
  slug: opper-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-system-api-openapi.yml
- filename: opper-tools-api-openapi.yml
  format: yaml
  label: Opper AI Tools API
  slug: opper-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-tools-api-openapi.yml
- filename: opper-traces-api-openapi.yml
  format: yaml
  label: Opper AI Traces API
  slug: opper-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-traces-api-openapi.yml
- filename: opper-user-delegation-api-openapi.yml
  format: yaml
  label: Opper AI User delegation API
  slug: opper-user-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-user-delegation-api-openapi.yml
- filename: opper-videos-api-openapi.yml
  format: yaml
  label: Opper AI Videos API
  slug: opper-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-videos-api-openapi.yml
auth_types: []
description: Authentication schemes for Opper AI
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Opper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opper AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Opper AI
provider_slug: opper
scheme_count: 2
schemes:
- evidence: 'description: API key authentication. Pass your API key as a Bearer token.'
  header: Authorization
  location: header
  name: BearerAuth
  type: http-bearer
- evidence: 'description: Management API authentication. Pass an `op-mak-…` management token as a Bearer token.'
  header: Authorization
  how_to_obtain: Mint a management key from the platform UI under Settings → API keys.
  location: header
  name: ManagementBearer
  type: http-bearer
slug: opper-authentication
source_filename: opper-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.opper.ai/v3-api-reference/management/list-api-keys.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.opper.ai/v3-api-reference/management/list-api-keys.md\nsources:\n- https://docs.opper.ai/v3-api-reference/management/list-api-keys.md\n- https://docs.opper.ai/v3-api-reference/management/create-api-key.md\n- https://docs.opper.ai/v3-api-reference/management/delete-api-key.md\n- https://docs.opper.ai/v3-api-reference/compatibility/count-message-tokens.md\ndescription: Authentication schemes for Opper AI\nschemes:\n- type: http-bearer\n  name: BearerAuth\n  evidence: 'description: API key authentication. Pass your API key as a Bearer token.'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: ManagementBearer\n  evidence: 'description: Management API authentication. Pass an `op-mak-…` management token as a Bearer token.'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a management key from the platform UI under Settings → API\
  \ keys.\ndocs: https://docs.opper.ai/v3-api-reference/management/list-api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/authentication/opper-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Gateway
- European
- OpenAI-compatible
- GDPR
---
