---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firstpromoter.com
  spf: true
hosts:
- cert_expires: Oct  4 10:07:09 2026 GMT
  host: firstpromoter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 10:07:09 2026 GMT
  host: docs.firstpromoter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 10:07:09 2026 GMT
  host: api.firstpromoter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firstpromoter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FirstPromoter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FirstPromoter
provider_slug: firstpromoter
slug: firstpromoter-domain-security
source_filename: firstpromoter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstpromoter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.firstpromoter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.firstpromoter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: firstpromoter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/security/firstpromoter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Referral Tracking
- SaaS
- Commission Management
- Reward Distribution
- Promoters
---
