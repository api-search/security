---
api_key_in: []
api_specs:
- filename: availity-auth-attachments-api-openapi.yml
  format: yaml
  label: availity Auth Attachments API
  slug: availity-auth-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-auth-attachments-api-openapi.yml
- filename: availity-claim-attachments-api-openapi.yml
  format: yaml
  label: availity Claim Attachments API
  slug: availity-claim-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-attachments-api-openapi.yml
- filename: availity-claim-status-api-openapi.yml
  format: yaml
  label: availity Claim Status API
  slug: availity-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-status-api-openapi.yml
- filename: availity-eligibility-api-openapi.yml
  format: yaml
  label: availity Eligibility API
  slug: availity-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-eligibility-api-openapi.yml
- filename: availity-enhanced-claim-status-api-openapi.yml
  format: yaml
  label: availity Enhanced Claim Status API
  slug: availity-enhanced-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-enhanced-claim-status-api-openapi.yml
- filename: availity-is-auth-required-api-openapi.yml
  format: yaml
  label: availity Is Auth Required API
  slug: availity-is-auth-required-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-is-auth-required-api-openapi.yml
- filename: availity-service-reviews-api-openapi.yml
  format: yaml
  label: availity Service Reviews API
  slug: availity-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-service-reviews-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Availity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Availity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Availity
provider_slug: availity
scheme_count: 1
schemes:
- declared_in:
  - openapi/_harvested/availity-aws-payer-list-swagger.json
  - openapi/_harvested/availity-care-cost-estimator-institutional-swagger.json
  - openapi/_harvested/availity-care-cost-estimator-professional-swagger.json
  - openapi/_harvested/availity-claim-statuses-swagger.json
  - openapi/_harvested/availity-configurations-swagger.json
  - openapi/_harvested/availity-coverages-swagger.json
  - openapi/_harvested/availity-dental-claims-swagger.json
  - openapi/_harvested/availity-dfs-swagger.json
  - openapi/_harvested/availity-patient-cost-estimator-professional-swagger.json
  - openapi/_harvested/availity-payer-list-swagger.json
  - openapi/_harvested/availity-service-reviews-swagger.json
  description: Application-only authentication based on the OAuth 2.0 Client Credentials Grant. This is the only authentication method Availity's public REST APIs support, including for demo/sandbox resources.
  flows:
  - call_pattern: 'Authorization: Bearer <access_token>'
    flow: clientCredentials
    tokenUrl: https://api.availity.com/v1/token
    token_request:
      case_sensitive: true
      content_type: application/x-www-form-urlencoded
      method: POST
      note: Availity explicitly warns that the request body parameter names and values are case sensitive.
      parameters:
      - name: grant_type
        required: true
        value: client_credentials
      - name: client_id
        required: true
        value: your API key (from the registered application in the developer portal)
      - name: client_secret
        required: true
        value: your client secret
      - name: scope
        required: true
        value: space-separated product and plan scopes, e.g. "healthcare-hipaa-transactions healthcare-hipaa-transactions-demo"
    token_response:
      expires_in: 300
      fields:
      - access_token
      - token_type
      - expires_in
      - scope
      - consented_on
      token_type: Bearer
  name: oauth2
  scopes_ref: scopes/availity-scopes.yml
  type: oauth2
slug: availity-authentication
source_filename: availity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developer.availity.com/blog/2025/3/25/availity-api-guide (Authentication + Availity API workflow sections), openapi/_harvested/*-swagger.json\ndocs: https://developer.availity.com/blog/2025/3/25/availity-api-guide\nprovider: Availity\nproviderId: availity\nsupersedes: >-\n  The previous derived version (2026-07-11) recorded tokenUrl\n  https://api.availity.com/availity/v1/token, read from hand-authored specs. Availity's own\n  published documents give https://api.availity.com/v1/token — corrected here from both the API\n  Guide cURL example and the securityDefinitions.oauth2.tokenUrl of all eleven harvested Swagger\n  documents.\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - clientCredentials\n  user_auth: false\n  mtls: false\n  api_key_direct: false\nschemes:\n  - name: oauth2\n    type: oauth2\n    description: >-\n      Application-only authentication based on the OAuth 2.0 Client Credentials Grant. This\
  \ is the\n      only authentication method Availity's public REST APIs support, including for demo/sandbox\n      resources.\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.availity.com/v1/token\n        token_request:\n          method: POST\n          content_type: application/x-www-form-urlencoded\n          parameters:\n            - name: grant_type\n              value: client_credentials\n              required: true\n            - name: client_id\n              value: your API key (from the registered application in the developer portal)\n              required: true\n            - name: client_secret\n              value: your client secret\n              required: true\n            - name: scope\n              value: 'space-separated product and plan scopes, e.g. \"healthcare-hipaa-transactions healthcare-hipaa-transactions-demo\"'\n              required: true\n          case_sensitive: true\n          note: >-\n            Availity explicitly warns\
  \ that the request body parameter names and values are case\n            sensitive.\n        token_response:\n          fields:\n            - access_token\n            - token_type\n            - expires_in\n            - scope\n            - consented_on\n          token_type: Bearer\n          expires_in: 300\n        call_pattern: 'Authorization: Bearer <access_token>'\n    scopes_ref: scopes/availity-scopes.yml\n    declared_in:\n      - openapi/_harvested/availity-aws-payer-list-swagger.json\n      - openapi/_harvested/availity-care-cost-estimator-institutional-swagger.json\n      - openapi/_harvested/availity-care-cost-estimator-professional-swagger.json\n      - openapi/_harvested/availity-claim-statuses-swagger.json\n      - openapi/_harvested/availity-configurations-swagger.json\n      - openapi/_harvested/availity-coverages-swagger.json\n      - openapi/_harvested/availity-dental-claims-swagger.json\n      - openapi/_harvested/availity-dfs-swagger.json\n      - openapi/_harvested/availity-patient-cost-estimator-professional-swagger.json\n\
  \      - openapi/_harvested/availity-payer-list-swagger.json\n      - openapi/_harvested/availity-service-reviews-swagger.json\ntoken_lifetime:\n  seconds: 300\n  minutes: 5\n  refresh_token: false\n  operational_note: >-\n    Five minutes is short. Availity issues no refresh token — the client re-runs the client\n    credentials grant. Any agent or batch job running longer than five minutes must re-authenticate\n    mid-run, and a 401 in the middle of a working session should be interpreted as an expired token\n    before it is interpreted as a credential problem. Token acquisition itself is not documented as\n    exempt from the rate limit, so a naive per-request token fetch burns plan quota.\nonboarding:\n  self_serve_to_demo: true\n  self_serve_to_production: false\n  steps:\n    - Create an account at developer.availity.com (email verification + mandatory MFA via an authenticator app).\n    - Create an Organization. Adding users to an organization requires a support ticket with case\
  \ reason \"API\".\n    - Register an application under My Apps to obtain the API key / client secret.\n    - Subscribe to an API product and choose a plan. Demo subscriptions are auto-approved.\n    - For the Standard plan, submit the portal request AND contact sales; Trading Partner Management completes contracting before activation.\n  gate: >-\n    Production access is sales-gated and contract-gated. The Demo plan is genuinely self-serve.\ntransport_security:\n  tls_required: true\n  note: >-\n    \"All Availity REST APIs support OAuth 2.0 over HTTPS for authentication.\" Every harvested\n    Swagger declares schemes: [https] only. See security/availity-domain-security.yml for the TLS\n    /HSTS/DNSSEC/CAA/SPF/DMARC probe.\nrelated_headers:\n  - name: X-Availity-Customer-Id\n    purpose: Identifies the customer organization on whose behalf the call is made.\n  - name: X-Response-Encoding-Context\n    purpose: Opt-in contextual output encoding (XSS mitigation). See conventions/availity-conventions.yml.\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/authentication/availity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Healthcare
- Clearinghouse
- HIPAA
- X12 EDI
- Eligibility
- Claims
- Prior Authorization
- Revenue Cycle Management
- Payers
- Price Transparency
---
