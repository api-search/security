---
anonymous_access: false
api_key_in: []
api_specs:
- filename: auto-reader-com-ask-api-openapi.yml
  format: yaml
  label: Auto Reader Ask API
  slug: auto-reader-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-ask-api-openapi.yml
- filename: auto-reader-com-book-api-openapi.yml
  format: yaml
  label: Auto Reader Book API
  slug: auto-reader-com-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-book-api-openapi.yml
- filename: auto-reader-com-correct-api-openapi.yml
  format: yaml
  label: Auto Reader Correct API
  slug: auto-reader-com-correct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-correct-api-openapi.yml
- filename: auto-reader-com-data-api-openapi.yml
  format: yaml
  label: Auto Reader Data API
  slug: auto-reader-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-data-api-openapi.yml
- filename: auto-reader-com-detect-api-openapi.yml
  format: yaml
  label: Auto Reader Detect API
  slug: auto-reader-com-detect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-detect-api-openapi.yml
- filename: auto-reader-com-document-api-openapi.yml
  format: yaml
  label: Auto Reader Document API
  slug: auto-reader-com-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-document-api-openapi.yml
- filename: auto-reader-com-export-api-openapi.yml
  format: yaml
  label: Auto Reader Export API
  slug: auto-reader-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-export-api-openapi.yml
- filename: auto-reader-com-extract-api-openapi.yml
  format: yaml
  label: Auto Reader Extract API
  slug: auto-reader-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-extract-api-openapi.yml
- filename: auto-reader-com-feedback-api-openapi.yml
  format: yaml
  label: Auto Reader Feedback API
  slug: auto-reader-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-feedback-api-openapi.yml
- filename: auto-reader-com-glossary-api-openapi.yml
  format: yaml
  label: Auto Reader Glossary API
  slug: auto-reader-com-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-glossary-api-openapi.yml
- filename: auto-reader-com-health-api-openapi.yml
  format: yaml
  label: Auto Reader Health API
  slug: auto-reader-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-health-api-openapi.yml
- filename: auto-reader-com-internal-api-openapi.yml
  format: yaml
  label: Auto Reader Internal API
  slug: auto-reader-com-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-internal-api-openapi.yml
- filename: auto-reader-com-jobs-api-openapi.yml
  format: yaml
  label: Auto Reader Jobs API
  slug: auto-reader-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-jobs-api-openapi.yml
- filename: auto-reader-com-manga-api-openapi.yml
  format: yaml
  label: Auto Reader Manga API
  slug: auto-reader-com-manga-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-manga-api-openapi.yml
- filename: auto-reader-com-ocr-api-openapi.yml
  format: yaml
  label: Auto Reader Ocr API
  slug: auto-reader-com-ocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-ocr-api-openapi.yml
- filename: auto-reader-com-ocr-translate-api-openapi.yml
  format: yaml
  label: Auto Reader Ocr Translate API
  slug: auto-reader-com-ocr-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-ocr-translate-api-openapi.yml
- filename: auto-reader-com-reduce-api-openapi.yml
  format: yaml
  label: Auto Reader Reduce API
  slug: auto-reader-com-reduce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-reduce-api-openapi.yml
- filename: auto-reader-com-rewrite-api-openapi.yml
  format: yaml
  label: Auto Reader Rewrite API
  slug: auto-reader-com-rewrite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-rewrite-api-openapi.yml
- filename: auto-reader-com-translate-api-openapi.yml
  format: yaml
  label: Auto Reader Translate API
  slug: auto-reader-com-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-translate-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Auto Reader Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Auto Reader secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Auto Reader
provider_slug: auto-reader-com
scheme_count: 1
schemes:
- description: API key from POST /signup (nsk_live_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/auto-reader-com.json
  type: http
slug: auto-reader-com-authentication
source_filename: auto-reader-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/auto-reader-com.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from POST /signup (nsk_live_...)\n  sources:\n  - openapi/auto-reader-com.json\n"
source_yaml_url: https://artifacts.apis.io/auto-reader-com/authentication/auto-reader-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Mobile
- Accessibility
- Audio
- eBook
- Offline
---
