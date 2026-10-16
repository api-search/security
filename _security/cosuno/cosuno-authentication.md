---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cosuno-awarded-bids-api-openapi.yml
  format: yaml
  label: Cosuno Awarded Bids API
  slug: cosuno-awarded-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-awarded-bids-api-openapi.yml
- filename: cosuno-bid-package-custom-fields-api-openapi.yml
  format: yaml
  label: Cosuno Bid Package Custom Fields API
  slug: cosuno-bid-package-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bid-package-custom-fields-api-openapi.yml
- filename: cosuno-bid-packages-api-openapi.yml
  format: yaml
  label: Cosuno Bid Packages API
  slug: cosuno-bid-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bid-packages-api-openapi.yml
- filename: cosuno-bid-requests-api-openapi.yml
  format: yaml
  label: Cosuno Bid Requests API
  slug: cosuno-bid-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bid-requests-api-openapi.yml
- filename: cosuno-bids-api-openapi.yml
  format: yaml
  label: Cosuno Bids API
  slug: cosuno-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-bids-api-openapi.yml
- filename: cosuno-company-api-openapi.yml
  format: yaml
  label: Cosuno Company API
  slug: cosuno-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-company-api-openapi.yml
- filename: cosuno-current-user-api-openapi.yml
  format: yaml
  label: Cosuno Current User API
  slug: cosuno-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-current-user-api-openapi.yml
- filename: cosuno-offices-api-openapi.yml
  format: yaml
  label: Cosuno Offices API
  slug: cosuno-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-offices-api-openapi.yml
- filename: cosuno-project-costs-api-openapi.yml
  format: yaml
  label: Cosuno Project Costs API
  slug: cosuno-project-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-project-costs-api-openapi.yml
- filename: cosuno-project-custom-fields-api-openapi.yml
  format: yaml
  label: Cosuno Project Custom Fields API
  slug: cosuno-project-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-project-custom-fields-api-openapi.yml
- filename: cosuno-projects-api-openapi.yml
  format: yaml
  label: Cosuno Projects API
  slug: cosuno-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-projects-api-openapi.yml
- filename: cosuno-subcontractor-custom-fields-api-openapi.yml
  format: yaml
  label: Cosuno Subcontractor Custom Fields API
  slug: cosuno-subcontractor-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-subcontractor-custom-fields-api-openapi.yml
- filename: cosuno-subcontractor-reviews-api-openapi.yml
  format: yaml
  label: Cosuno Subcontractor Reviews API
  slug: cosuno-subcontractor-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-subcontractor-reviews-api-openapi.yml
- filename: cosuno-subcontractors-api-openapi.yml
  format: yaml
  label: Cosuno Subcontractors API
  slug: cosuno-subcontractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-subcontractors-api-openapi.yml
- filename: cosuno-users-api-openapi.yml
  format: yaml
  label: Cosuno Users API
  slug: cosuno-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-users-api-openapi.yml
- filename: cosuno-webhooks-api-openapi.yml
  format: yaml
  label: Cosuno Webhooks API
  slug: cosuno-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-webhooks-api-openapi.yml
- filename: cosuno-work-categories-api-openapi.yml
  format: yaml
  label: Cosuno Work Categories API
  slug: cosuno-work-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/openapi/cosuno-work-categories-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cosuno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosuno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cosuno
provider_slug: cosuno
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cosuno-openapi.json
  type: http
slug: cosuno-authentication
source_filename: cosuno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: derived\nsource: openapi/cosuno-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cosuno-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosuno/refs/heads/main/authentication/cosuno-authentication.yml
summary_line: http · 1 scheme
tags:
- Construction
- Marketplace
- AI
- Tendering
- Germany
---
