---
api_key_in:
- header
api_specs:
- filename: apyhub-artificial-intelligence-api-openapi.yml
  format: yaml
  label: ApyHub Artificial Intelligence API
  slug: apyhub-artificial-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-artificial-intelligence-api-openapi.yml
- filename: apyhub-audio-processing-api-openapi.yml
  format: yaml
  label: ApyHub Audio Processing API
  slug: apyhub-audio-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-audio-processing-api-openapi.yml
- filename: apyhub-communications-api-openapi.yml
  format: yaml
  label: ApyHub Communications API
  slug: apyhub-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-communications-api-openapi.yml
- filename: apyhub-data-extraction-api-openapi.yml
  format: yaml
  label: ApyHub Data Extraction API
  slug: apyhub-data-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-data-extraction-api-openapi.yml
- filename: apyhub-data-validation-api-openapi.yml
  format: yaml
  label: ApyHub Data Validation API
  slug: apyhub-data-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-data-validation-api-openapi.yml
- filename: apyhub-developer-tools-api-openapi.yml
  format: yaml
  label: ApyHub Developer Tools API
  slug: apyhub-developer-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-developer-tools-api-openapi.yml
- filename: apyhub-e-commerce-quick-tools-api-openapi.yml
  format: yaml
  label: ApyHub E-commerce Quick Tools API
  slug: apyhub-e-commerce-quick-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-e-commerce-quick-tools-api-openapi.yml
- filename: apyhub-file-conversion-api-openapi.yml
  format: yaml
  label: ApyHub File Conversion API
  slug: apyhub-file-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-file-conversion-api-openapi.yml
- filename: apyhub-file-manipulation-api-openapi.yml
  format: yaml
  label: ApyHub File Manipulation API
  slug: apyhub-file-manipulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-file-manipulation-api-openapi.yml
- filename: apyhub-file-security-api-openapi.yml
  format: yaml
  label: ApyHub File Security API
  slug: apyhub-file-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-file-security-api-openapi.yml
- filename: apyhub-finance-api-openapi.yml
  format: yaml
  label: ApyHub Finance API
  slug: apyhub-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-finance-api-openapi.yml
- filename: apyhub-geolocation-api-openapi.yml
  format: yaml
  label: ApyHub Geolocation API
  slug: apyhub-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-geolocation-api-openapi.yml
- filename: apyhub-hr-api-openapi.yml
  format: yaml
  label: ApyHub HR API
  slug: apyhub-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-hr-api-openapi.yml
- filename: apyhub-marketing-api-openapi.yml
  format: yaml
  label: ApyHub Marketing API
  slug: apyhub-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-marketing-api-openapi.yml
- filename: apyhub-security-privacy-api-openapi.yml
  format: yaml
  label: ApyHub Security & Privacy API
  slug: apyhub-security-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-security-privacy-api-openapi.yml
- filename: apyhub-seo-api-openapi.yml
  format: yaml
  label: ApyHub SEO API
  slug: apyhub-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-seo-api-openapi.yml
- filename: apyhub-smart-generation-api-openapi.yml
  format: yaml
  label: ApyHub Smart Generation API
  slug: apyhub-smart-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-smart-generation-api-openapi.yml
- filename: apyhub-standard-data-api-openapi.yml
  format: yaml
  label: ApyHub Standard Data API
  slug: apyhub-standard-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-standard-data-api-openapi.yml
- filename: apyhub-uncategorized-api-openapi.yml
  format: yaml
  label: ApyHub Uncategorized API
  slug: apyhub-uncategorized-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-uncategorized-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apyhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: ApyHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ApyHub
provider_slug: apyhub
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: apy-token
  sources:
  - openapi/apyhub-openapi.yaml
  type: apiKey
slug: apyhub-authentication
source_filename: apyhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apyhub-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apy-token\n  sources:\n  - openapi/apyhub-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/authentication/apyhub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Marketplace
- API Platform
- Utility APIs
- Document Conversion
- Data Processing
- Artificial Intelligence
- MCP
- Agent Ready
---
