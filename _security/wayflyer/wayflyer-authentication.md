---
api_key_in: []
api_specs:
- filename: wayflyer-embedded-finance-openapi-original.json
  format: json
  label: Wayflyer Embedded Finance API
  slug: embedded-finance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-embedded-finance-openapi-original.json
- filename: wayflyer-embedded-finance-sandbox-openapi-original.json
  format: json
  label: Wayflyer Embedded Finance Sandbox API
  slug: embedded-finance-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/openapi/wayflyer-embedded-finance-sandbox-openapi-original.json
auth_types:
- http
description: 'Authentication profile for the Wayflyer Embedded Finance (Hosted Capital) API. Two-tier bearer-JWT model: partners exchange a backend-only client_id/client_secret for a Partner Token, then mint per-merchant Company Tokens that are forwarded to the frontend for SDK / API calls. Both token classes appear in the OpenAPI as http bearer securitySchemes (PartnerToken, CompanyToken). No OAuth2/OIDC flows and no API-key scheme; the sandbox environment uses a separate sandbox client_id/secret.'
kind: authentication
layout: security
method: searched
name: Wayflyer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wayflyer secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wayflyer
provider_slug: wayflyer
scheme_count: 2
schemes:
- name: CompanyToken
  scheme: bearer
  sources:
  - openapi/wayflyer-embedded-finance-openapi-original.json
  - openapi/wayflyer-embedded-finance-sandbox-openapi-original.json
  type: http
- name: PartnerToken
  scheme: bearer
  sources:
  - openapi/wayflyer-embedded-finance-openapi-original.json
  - openapi/wayflyer-embedded-finance-sandbox-openapi-original.json
  type: http
slug: wayflyer-authentication
source_filename: wayflyer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.wayflyer.com/embedded-journey-v5-overview/shared/authentication\ndocs: https://docs.wayflyer.com/embedded-journey-v5-overview/shared/authentication\ndescription: >-\n  Authentication profile for the Wayflyer Embedded Finance (Hosted Capital)\n  API. Two-tier bearer-JWT model: partners exchange a backend-only\n  client_id/client_secret for a Partner Token, then mint per-merchant Company\n  Tokens that are forwarded to the frontend for SDK / API calls. Both token\n  classes appear in the OpenAPI as http bearer securitySchemes (PartnerToken,\n  CompanyToken). No OAuth2/OIDC flows and no API-key scheme; the sandbox\n  environment uses a separate sandbox client_id/secret.\nsummary:\n  types: [http]\n  schemes: [bearer]\n  oauth2_flows: []\ncredentials:\n  issued: client_id + client_secret at partner onboarding (backend-only; never expose in the frontend)\ntoken_model:\n  - name: PartnerToken\n    obtain: POST https://api.wayflyer.com/financing/v1/partner-token/\n\
  \    payload: '{\"partner_id\": \"<client_id>\", \"partner_secret\": \"<client_secret>\"}'\n    format: JWT\n    header: 'Authorization: Bearer <token>'\n    expires_in: 86000\n    caching: securely cache and re-use until expiry\n    used_for: partner-scope operations (company-token minting, anonymized data uploads)\n  - name: CompanyToken\n    obtain: POST https://api.wayflyer.com/financing/v1/partner/company-token/ (authenticated with PartnerToken)\n    payload: '{\"company_id\": \"<anonymous-string-id>\", \"user_id\": \"<user-id>\"}'\n    format: JWT\n    header: 'Authorization: Bearer <token>'\n    expires_in: 86000\n    used_for: all company-scope operations (CTA, applications, details, documents); forwarded to the frontend for the SDKs\n    company_id_rules: anonymous, consistent, unique per company, string < 255 chars, must not reveal identity without consent\nschemes:\n  - name: CompanyToken\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/wayflyer-embedded-finance-openapi-original.json\n\
  \      - openapi/wayflyer-embedded-finance-sandbox-openapi-original.json\n  - name: PartnerToken\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/wayflyer-embedded-finance-openapi-original.json\n      - openapi/wayflyer-embedded-finance-sandbox-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayflyer/refs/heads/main/authentication/wayflyer-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Ecommerce
- Fintech
- Embedded Finance
- Lending
- Revenue-Based Financing
- Financing
---
