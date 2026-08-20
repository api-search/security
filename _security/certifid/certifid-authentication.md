---
api_key_in: []
api_specs:
- filename: certifid-accountverifications-api-openapi.yml
  format: yaml
  label: CertifID Account Verifications API
  slug: certifid-accountverifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-accountverifications-api-openapi.yml
- filename: certifid-banklookup-api-openapi.yml
  format: yaml
  label: CertifID Bank Lookup API
  slug: certifid-banklookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-banklookup-api-openapi.yml
- filename: certifid-collectrequest-api-openapi.yml
  format: yaml
  label: CertifID Collect Request API
  slug: certifid-collectrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-collectrequest-api-openapi.yml
- filename: certifid-confirmrequest-api-openapi.yml
  format: yaml
  label: CertifID Confirm Request API
  slug: certifid-confirmrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-confirmrequest-api-openapi.yml
- filename: certifid-disbursements-api-openapi.yml
  format: yaml
  label: CertifID Disbursements API
  slug: certifid-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-disbursements-api-openapi.yml
- filename: certifid-identityrequest-api-openapi.yml
  format: yaml
  label: CertifID Identity Request API
  slug: certifid-identityrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-identityrequest-api-openapi.yml
- filename: certifid-integration-api-openapi.yml
  format: yaml
  label: CertifID Integration API
  slug: certifid-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-integration-api-openapi.yml
- filename: certifid-lenders-api-openapi.yml
  format: yaml
  label: CertifID Lenders API
  slug: certifid-lenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-lenders-api-openapi.yml
- filename: certifid-location-api-openapi.yml
  format: yaml
  label: CertifID Location API
  slug: certifid-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-location-api-openapi.yml
- filename: certifid-payoffordering-api-openapi.yml
  format: yaml
  label: CertifID Payoff Ordering API
  slug: certifid-payoffordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-payoffordering-api-openapi.yml
- filename: certifid-sendrequest-api-openapi.yml
  format: yaml
  label: CertifID Send Request API
  slug: certifid-sendrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-sendrequest-api-openapi.yml
- filename: certifid-test-api-openapi.yml
  format: yaml
  label: CertifID Test API
  slug: certifid-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-test-api-openapi.yml
- filename: certifid-underwriter-api-openapi.yml
  format: yaml
  label: CertifID Underwriter API
  slug: certifid-underwriter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-underwriter-api-openapi.yml
- filename: certifid-users-api-openapi.yml
  format: yaml
  label: CertifID Users API
  slug: certifid-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-users-api-openapi.yml
- filename: certifid-wiringinstructions-api-openapi.yml
  format: yaml
  label: CertifID Wiring Instructions API
  slug: certifid-wiringinstructions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-wiringinstructions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Certifid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CertifID secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CertifID
provider_slug: certifid
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.certifid.com/authorize?audience=https://api.certifid.com&connection=CertifID-Users-DB
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.certifid.com/oauth/token
  name: oauth2
  sources:
  - openapi/certifid-v2-apis-openapi.json
  type: oauth2
slug: certifid-authentication
source_filename: certifid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/certifid-v2-apis-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.certifid.com/authorize?audience=https://api.certifid.com&connection=CertifID-Users-DB\n    tokenUrl: https://auth.certifid.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/authentication/certifid-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Wire Fraud Prevention
- Real-Estate
- Title Insurance
- Identity Verification
- Business Verification
- Payments
- Fraud Prevention
- Escrow and Settlement
- Financial-Services
- Security
---
