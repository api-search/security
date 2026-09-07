---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Acorn Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acorn Finance declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Acorn Finance
provider_slug: acorn-finance
scheme_count: 1
schemes:
- applies_to: all documented endpoints
  description: HTTP Basic authentication is the only mechanism Acorn Finance documents. A username/password credential pair is issued per partner company, separately for production and for the UAT testing environment. Every documented endpoint requires it; there is no anonymous surface.
  evidence: '"We use Basic Authorization. We will create your credentials for Production and Testing" — https://docs.acornfinance.com/api-sign-up'
  format: 'Authorization: Basic <base64(username:password)>'
  header: Authorization
  id: basic
  in: header
  scheme: basic
  type: http
slug: acorn-finance-authentication
source_filename: acorn-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.acornfinance.com/api-sign-up\ndocs:\n- https://docs.acornfinance.com/api-sign-up\n- https://docs.acornfinance.com/api-active-credential\n- https://docs.acornfinance.com/api-company-user\nnote: >-\n  Derived by reading the Acorn Finance partner documentation directly. Acorn Finance\n  publishes no OpenAPI document, so there are no securitySchemes to parse; the model\n  below is transcribed from the provider's own \"API Authorization\" and \"API Active\n  Credentials\" pages.\napi: Acorn Finance Partner API\nbase_urls:\n  production: https://api.acornfinance.com\n  testing: https://uat.api.acornfinance.com\nschemes:\n- id: basic\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  format: 'Authorization: Basic <base64(username:password)>'\n  description: >-\n    HTTP Basic authentication is the only mechanism Acorn Finance documents. A\n    username/password credential pair is issued per partner\
  \ company, separately for\n    production and for the UAT testing environment. Every documented endpoint\n    requires it; there is no anonymous surface.\n  applies_to: all documented endpoints\n  evidence: >-\n    \"We use Basic Authorization. We will create your credentials for Production and\n    Testing\" — https://docs.acornfinance.com/api-sign-up\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key_header: false\nonboarding:\n  self_service: false\n  steps:\n  - Sign your company up for Acorn Finance at https://sign-up.acornfinance.com/\n  - Email it@acornfinance.com with subject \"Create API Credentials\" and your company\n    name in the body\n  turnaround: within 48 hours Monday-Friday\n  issued_by_provider:\n  - production API credentials\n  - testing (UAT) API credentials\n  - a Dealer Id prefix (for example QRS- for the documented sample partner)\n  - app_company_parent_id and parent_company_name, when the partner creates child\n    companies\n  evidence: https://docs.acornfinance.com/api-sign-up\n\
  credential_rotation:\n  supported: true\n  interval_days: 90\n  policy: >-\n    Acorn Finance rotates partner API credentials every 90 days. The provider states\n    this is a security requirement, not an option.\n  discovery_endpoint:\n    method: GET\n    production: https://api.acornfinance.com/active_credentials\n    testing: https://uat.api.acornfinance.com/active_credentials\n    description: >-\n      Returns the currently active credential pair for the calling company. Called\n      with the OLD credential, it returns the new one once it has been created;\n      if a new key has not yet been created it returns the old key unchanged.\n    response_fields:\n    - username\n    - password\n    - created_at\n    - expires_on\n    requirements:\n    - the old key must still be active\n    - the latest active key must have been created\n    - the company must be active\n  evidence: https://docs.acornfinance.com/api-active-credential\nfailure_modes:\n- status: 403\n  body: '{\"errors\"\
  : [\"Invalid Credentials\"]}'\n  cause: company inactive, or the key used for Basic auth is inactive\n- status: 422\n  body: '{\"errors\": [\"Missing Data\"]}'\n  cause: required request attributes absent\nsupport_contact: it@acornfinance.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acorn-finance/refs/heads/main/authentication/acorn-finance-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Financial Services
- Lending
- Loans
- Home Improvement
- Embedded Finance
- Point of Sale
- Consumer Finance
- Fintech
- Webhooks
---
