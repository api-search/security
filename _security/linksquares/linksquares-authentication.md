---
api_key_in: []
api_specs:
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Analyze Agreements API
  slug: linksquares-analyze-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Analyze Metadata and Smart Values API
  slug: linksquares-analyze-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Finalize Workflow API
  slug: linksquares-finalize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Linksquares Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkSquares secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LinkSquares
provider_slug: linksquares
scheme_count: 1
schemes:
- description: LinkSquares APIs use API key authentication. The API key is a unique alphanumeric string that identifies your company's data, and it must be included as an `x-api-key` header on every request. The same token is shared across the Analyze and Finalize products and can interact with either application. Behind the gateway, LinkSquares additionally issues JWTs (JSON Web Tokens) as part of request handling, but callers only supply the x-api-key header. Keys are self-managed by Administrator users via the LinkSquares application, are scoped to the managing user account's permissions, and should be treated as secret since access is equivalent to access to your agreements. User and group provisioning is handled separately via SCIM 2.0 on the Enterprise tier.
  in: header
  name: apiKeyAuth
  parameterName: x-api-key
  sources:
  - https://help.linksquares.com/hc/en-us/articles/10575849523735-Managing-API-Keys
  - https://help.linksquares.com/hc/en-us/articles/10575707057175-LinkSquares-API-Overview
  type: apiKey
slug: linksquares-authentication
source_filename: linksquares-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: openapi/linksquares-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: x-api-key\n  description: >-\n    LinkSquares APIs use API key authentication. The API key is a unique\n    alphanumeric string that identifies your company's data, and it must be\n    included as an `x-api-key` header on every request. The same token is shared\n    across the Analyze and Finalize products and can interact with either\n    application. Behind the gateway, LinkSquares additionally issues JWTs (JSON\n    Web Tokens) as part of request handling, but callers only supply the\n    x-api-key header. Keys are self-managed by Administrator users via the\n    LinkSquares application, are scoped to the managing user account's\n    permissions, and should be treated as secret since access is equivalent to\n    access to your agreements. User and group provisioning is handled separately\n\
  \    via SCIM 2.0 on the Enterprise tier.\n  sources:\n  - https://help.linksquares.com/hc/en-us/articles/10575849523735-Managing-API-Keys\n  - https://help.linksquares.com/hc/en-us/articles/10575707057175-LinkSquares-API-Overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/authentication/linksquares-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- AI
- Legal
- Agreements
- Document Management
- Contract Analytics
---
