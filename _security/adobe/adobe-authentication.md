---
api_key_in: []
api_specs:
- filename: adobe-accessibility-auto-tag-api-openapi.yml
  format: yaml
  label: Adobe Accessibility Auto-Tag API
  slug: adobe-accessibility-auto-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-accessibility-auto-tag-api-openapi.yml
- filename: adobe-assets-api-openapi.yml
  format: yaml
  label: Adobe Assets API
  slug: adobe-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-assets-api-openapi.yml
- filename: adobe-combine-pdf-api-openapi.yml
  format: yaml
  label: Adobe Combine PDF API
  slug: adobe-combine-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-combine-pdf-api-openapi.yml
- filename: adobe-compress-pdf-api-openapi.yml
  format: yaml
  label: Adobe Compress PDF API
  slug: adobe-compress-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-compress-pdf-api-openapi.yml
- filename: adobe-create-pdf-api-openapi.yml
  format: yaml
  label: Adobe Create PDF API
  slug: adobe-create-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-create-pdf-api-openapi.yml
- filename: adobe-delete-pages-api-openapi.yml
  format: yaml
  label: Adobe Delete Pages API
  slug: adobe-delete-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-delete-pages-api-openapi.yml
- filename: adobe-document-generation-api-openapi.yml
  format: yaml
  label: Adobe Document Generation API
  slug: adobe-document-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-document-generation-api-openapi.yml
- filename: adobe-export-pdf-api-openapi.yml
  format: yaml
  label: Adobe Export PDF API
  slug: adobe-export-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-export-pdf-api-openapi.yml
- filename: adobe-extract-pdf-api-openapi.yml
  format: yaml
  label: Adobe Extract PDF API
  slug: adobe-extract-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-extract-pdf-api-openapi.yml
- filename: adobe-insert-pages-api-openapi.yml
  format: yaml
  label: Adobe Insert Pages API
  slug: adobe-insert-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-insert-pages-api-openapi.yml
- filename: adobe-jobs-api-openapi.yml
  format: yaml
  label: Adobe Jobs API
  slug: adobe-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-jobs-api-openapi.yml
- filename: adobe-linearize-pdf-api-openapi.yml
  format: yaml
  label: Adobe Linearize PDF API
  slug: adobe-linearize-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-linearize-pdf-api-openapi.yml
- filename: adobe-ocr-api-openapi.yml
  format: yaml
  label: Adobe OCR API
  slug: adobe-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-ocr-api-openapi.yml
- filename: adobe-pdf-properties-api-openapi.yml
  format: yaml
  label: Adobe PDF Properties API
  slug: adobe-pdf-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-pdf-properties-api-openapi.yml
- filename: adobe-protect-pdf-api-openapi.yml
  format: yaml
  label: Adobe Protect PDF API
  slug: adobe-protect-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-protect-pdf-api-openapi.yml
- filename: adobe-remove-protection-api-openapi.yml
  format: yaml
  label: Adobe Remove Protection API
  slug: adobe-remove-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-remove-protection-api-openapi.yml
- filename: adobe-reorder-pages-api-openapi.yml
  format: yaml
  label: Adobe Reorder Pages API
  slug: adobe-reorder-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-reorder-pages-api-openapi.yml
- filename: adobe-replace-pages-api-openapi.yml
  format: yaml
  label: Adobe Replace Pages API
  slug: adobe-replace-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-replace-pages-api-openapi.yml
- filename: adobe-rotate-pages-api-openapi.yml
  format: yaml
  label: Adobe Rotate Pages API
  slug: adobe-rotate-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-rotate-pages-api-openapi.yml
- filename: adobe-split-pdf-api-openapi.yml
  format: yaml
  label: Adobe Split PDF API
  slug: adobe-split-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-split-pdf-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adobe
provider_slug: adobe
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via client credentials grant from Adobe Identity Management Service (IMS). Generate credentials in the Adobe Developer Console and exchange them for an access token at https://ims-na1.adobelogin.com/ims/token/v3.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-pdf-services-api-openapi.yml
  type: http
slug: adobe-authentication
source_filename: adobe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-pdf-services-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via client credentials grant from Adobe Identity\n    Management Service (IMS). Generate credentials in the Adobe Developer Console and exchange\n    them for an access token at https://ims-na1.adobelogin.com/ims/token/v3.\n  sources:\n  - openapi/adobe-pdf-services-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/authentication/adobe-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 1000
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
---
