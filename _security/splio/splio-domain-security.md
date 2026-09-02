---
api_specs:
- filename: TzRX9kyT
  format: yaml
  label: Splio Referral API
  slug: splio-referral-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/10206569/TzRX9kyT
- filename: splio-blacklist-api-openapi.yml
  format: yaml
  label: Splio Blacklist API
  slug: splio-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-blacklist-api-openapi.yml
- filename: splio-contact-api-openapi.yml
  format: yaml
  label: Splio Contact API
  slug: splio-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-contact-api-openapi.yml
- filename: splio-coupon-api-openapi.yml
  format: yaml
  label: Splio Coupon API
  slug: splio-coupon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-coupon-api-openapi.yml
- filename: splio-export-api-openapi.yml
  format: yaml
  label: Splio Export API
  slug: splio-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-export-api-openapi.yml
- filename: splio-fields-api-openapi.yml
  format: yaml
  label: Splio Fields API
  slug: splio-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-fields-api-openapi.yml
- filename: splio-filter-api-openapi.yml
  format: yaml
  label: Splio Filter API
  slug: splio-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-filter-api-openapi.yml
- filename: splio-general-api-openapi.yml
  format: yaml
  label: Splio General API
  slug: splio-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-general-api-openapi.yml
- filename: splio-group-api-openapi.yml
  format: yaml
  label: Splio Group API
  slug: splio-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-group-api-openapi.yml
- filename: splio-loyalty-api-openapi.yml
  format: yaml
  label: Splio Loyalty API
  slug: splio-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-loyalty-api-openapi.yml
- filename: splio-members-api-openapi.yml
  format: yaml
  label: Splio Members API
  slug: splio-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-members-api-openapi.yml
- filename: splio-one-shot-api-openapi.yml
  format: yaml
  label: Splio One Shot API
  slug: splio-one-shot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-one-shot-api-openapi.yml
- filename: splio-points-api-openapi.yml
  format: yaml
  label: Splio Points API
  slug: splio-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-points-api-openapi.yml
- filename: splio-programs-api-openapi.yml
  format: yaml
  label: Splio Programs API
  slug: splio-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-programs-api-openapi.yml
- filename: splio-reward-api-openapi.yml
  format: yaml
  label: Splio Reward API
  slug: splio-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-reward-api-openapi.yml
- filename: splio-reward-stock-and-codes-api-openapi.yml
  format: yaml
  label: Splio Reward stock and codes API
  slug: splio-reward-stock-and-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-reward-stock-and-codes-api-openapi.yml
- filename: splio-sales-data-api-openapi.yml
  format: yaml
  label: Splio Sales data API
  slug: splio-sales-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-sales-data-api-openapi.yml
- filename: splio-universe-api-openapi.yml
  format: yaml
  label: Splio Universe API
  slug: splio-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-universe-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:techops@splio.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: splio.com
  spf: true
hosts:
- cert_expires: Nov  8 00:42:56 2026 GMT
  host: splio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 04:48:43 2026 GMT
  host: dev-scp.splio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 02:03:33 2026 GMT
  host: api.splio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Splio
provider_slug: splio
slug: splio-domain-security
source_filename: splio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: splio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 00:42:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-scp.splio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 04:48:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.splio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 02:03:33 2026 GMT\n  hsts: null\ndomains:\n- domain: splio.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:techops@splio.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/security/splio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing Automation
- Customer Data Platform
- Loyalty
- CRM
- Email Marketing
- SMS
- Mobile Wallet
- Retail
- E-Commerce
- Predictive AI
- Customer Engagement
- France
---
