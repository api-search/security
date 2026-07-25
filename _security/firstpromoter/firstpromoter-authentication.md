---
api_key_in: []
api_specs:
- filename: firstpromoter-commissions-api-openapi.yml
  format: yaml
  label: FirstPromoter Commissions API
  slug: firstpromoter-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-commissions-api-openapi.yml
- filename: firstpromoter-company-api-openapi.yml
  format: yaml
  label: FirstPromoter Company API
  slug: firstpromoter-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-company-api-openapi.yml
- filename: firstpromoter-emails-api-openapi.yml
  format: yaml
  label: FirstPromoter Emails API
  slug: firstpromoter-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-emails-api-openapi.yml
- filename: firstpromoter-payouts-api-openapi.yml
  format: yaml
  label: FirstPromoter Payouts API
  slug: firstpromoter-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-payouts-api-openapi.yml
- filename: firstpromoter-promo-codes-api-openapi.yml
  format: yaml
  label: FirstPromoter Promo Codes API
  slug: firstpromoter-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-promo-codes-api-openapi.yml
- filename: firstpromoter-promoter-campaigns-api-openapi.yml
  format: yaml
  label: FirstPromoter Promoter Campaigns API
  slug: firstpromoter-promoter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-promoter-campaigns-api-openapi.yml
- filename: firstpromoter-promoters-api-openapi.yml
  format: yaml
  label: FirstPromoter Promoters API
  slug: firstpromoter-promoters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-promoters-api-openapi.yml
- filename: firstpromoter-referrals-api-openapi.yml
  format: yaml
  label: FirstPromoter Referrals API
  slug: firstpromoter-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-referrals-api-openapi.yml
- filename: firstpromoter-reports-api-openapi.yml
  format: yaml
  label: FirstPromoter Reports API
  slug: firstpromoter-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-reports-api-openapi.yml
- filename: firstpromoter-track-api-openapi.yml
  format: yaml
  label: FirstPromoter Track API
  slug: firstpromoter-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-track-api-openapi.yml
- filename: firstpromoter-webhook-deliveries-api-openapi.yml
  format: yaml
  label: FirstPromoter Webhook Deliveries API
  slug: firstpromoter-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-webhook-deliveries-api-openapi.yml
- filename: firstpromoter-webhooks-api-openapi.yml
  format: yaml
  label: FirstPromoter Webhooks API
  slug: firstpromoter-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Firstpromoter Authentication
name_suffix: Authentication
oauth_flows: []
overview: FirstPromoter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FirstPromoter
provider_slug: firstpromoter
scheme_count: 1
schemes:
- description: API key passed as Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/firstpromoter-firstpromoter-admin-api-openapi.yml
  type: http
slug: firstpromoter-authentication
source_filename: firstpromoter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/firstpromoter-firstpromoter-admin-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as Bearer token\n  sources:\n  - openapi/firstpromoter-firstpromoter-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/authentication/firstpromoter-authentication.yml
summary_line: http · 1 scheme
tags:
- Affiliate Marketing
- Referral Tracking
- SaaS
- Commission Management
- Reward Distribution
- Promoters
---
