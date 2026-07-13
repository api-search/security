---
api_specs:
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Checkout API
  slug: tabby-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Payments API
  slug: tabby-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Webhooks API
  slug: tabby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Disputes API
  slug: tabby-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tabby.ai
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: tabby.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:36:23 2026 GMT
  host: docs.tabby.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.tabby.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tabby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabby, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tabby
provider_slug: tabby
slug: tabby-domain-security
source_filename: tabby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tabby.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tabby.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:36:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tabby.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tabby.ai\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/security/tabby-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- BNPL
- Buy Now Pay Later
- Consumer Finance
- E-commerce
- Fintech
- Installments
- MENA
- Payments
- Saudi Arabia
- UAE
---
