---
api_specs:
- filename: openapi
  format: yaml
  label: GoCardless REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://developer.gocardless.com/api-reference/openapi
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:core-infrastructure-ext@gocardless.com"
  - 0 issue "actalis.it"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gocardless.com
  spf: true
hosts:
- cert_expires: Aug 27 02:05:31 2026 GMT
  host: gocardless.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:33:00 2026 GMT
  host: developer.gocardless.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:06:15 2026 GMT
  host: api.gocardless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gocardless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoCardless, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoCardless
provider_slug: gocardless
slug: gocardless-domain-security
source_filename: gocardless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gocardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:05:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: developer.gocardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:33:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.gocardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:06:15 2026 GMT\n  hsts: null\ndomains:\n- domain: gocardless.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:core-infrastructure-ext@gocardless.com\"\n  - 0 issue \"actalis.it\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/security/gocardless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Direct Debit
- Bank Debit
- Recurring Payments
- Subscriptions
- SEPA
- Bacs
- ACH
- Open Banking
- Fintech
---
