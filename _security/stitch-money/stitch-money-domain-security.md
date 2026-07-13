---
api_specs:
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Payments (Pay By Bank)
  slug: payments-pay-by-bank
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Account Verification API
  slug: account-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Financial Data API
  slug: financial-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Payouts and Disbursements API
  slug: payouts-disbursements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Refunds API
  slug: refunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Webhooks and Subscriptions API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stitch.money
  spf: true
hosts:
- cert_expires: Sep 30 20:13:01 2026 GMT
  host: stitch.money
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:30:22 2026 GMT
  host: docs.stitch.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:30:22 2026 GMT
  host: api.stitch.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stitch Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stitch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stitch
provider_slug: stitch-money
slug: stitch-money-domain-security
source_filename: stitch-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stitch.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:13:01 2026 GMT\n  hsts: false\n- host: docs.stitch.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stitch.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stitch.money\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/security/stitch-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Open Banking
- Pay By Bank
- GraphQL
- Africa
- South Africa
- Fintech
---
