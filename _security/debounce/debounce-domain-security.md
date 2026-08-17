---
api_specs:
- filename: debounce-validation-api-openapi.yml
  format: yaml
  label: DeBounce Validation API
  slug: debounce-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-validation-api-openapi.yml
- filename: debounce-bulk-api-openapi.yml
  format: yaml
  label: DeBounce Bulk API
  slug: debounce-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-bulk-api-openapi.yml
- filename: debounce-data-api-openapi.yml
  format: yaml
  label: DeBounce Data API
  slug: debounce-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-data-api-openapi.yml
- filename: debounce-account-api-openapi.yml
  format: yaml
  label: DeBounce Account API
  slug: debounce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-account-api-openapi.yml
- filename: debounce-disposable-api-openapi.yml
  format: yaml
  label: DeBounce Disposable Detector API
  slug: debounce-disposable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-disposable-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: debounce.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: debounce.io
  spf: true
hosts:
- cert_expires: Oct 15 22:47:55 2026 GMT
  host: debounce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 19:29:30 2026 GMT
  host: developers.debounce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 16:00:41 2026 GMT
  host: api.debounce.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 16:00:41 2026 GMT
  host: bulk.debounce.io
  hsts: null
  https: true
  source: manual probe — added 2026-08-14 for the bulk.debounce.io servers[] host
  tls_version: TLSv1.3
- cert_expires: Oct 29 16:00:41 2026 GMT
  host: disposable.debounce.io
  hsts: null
  https: true
  source: manual probe — added 2026-08-14 for the disposable.debounce.io servers[] host
  tls_version: TLSv1.3
- cert_expires: Oct 15 22:47:55 2026 GMT
  host: logo.debounce.com
  hsts: null
  https: true
  source: manual probe — added 2026-08-14 for the Logo API host
  tls_version: TLSv1.3
- cert_expires: Oct 29 16:00:41 2026 GMT
  host: app.debounce.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  source: manual probe — added 2026-08-14 for the signup/dashboard host
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Debounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeBounce, probed live across 7 host(s) and 2 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeBounce
provider_slug: debounce
slug: debounce-domain-security
source_filename: debounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: debounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:47:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.debounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.debounce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 16:00:41 2026 GMT\n  hsts: null\n- host: bulk.debounce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 16:00:41 2026 GMT\n  hsts: null\n  source: manual probe — added 2026-08-14 for the bulk.debounce.io servers[] host\n- host: disposable.debounce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 16:00:41 2026 GMT\n  hsts: null\n  source: manual probe — added 2026-08-14 for the disposable.debounce.io servers[] host\n- host: logo.debounce.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:47:55 2026 GMT\n  hsts: null\n  source: manual probe — added 2026-08-14 for the Logo API host\n- host: app.debounce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 16:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  source: manual probe — added 2026-08-14 for the signup/dashboard host\nfindings:\n- >-\n  HSTS is set on the marketing site (debounce.com), the developer portal\n  (developers.debounce.com, max-age 63072000 — the longest in the profile) and\n  the dashboard (app.debounce.io), but on NONE of the four API hosts:\n  api.debounce.io, bulk.debounce.io, disposable.debounce.io and\n  logo.debounce.com all answer without a Strict-Transport-Security header. Since\n  the API key travels in the query string, an API host without HSTS is the\n  weakest link in this profile.\n- >-\n  Neither registrable domain has DNSSEC enabled. debounce.com publishes no CAA\n  record at all; debounce.io does.\n- >-\n  Both domains\
  \ publish SPF and a DMARC policy of p=reject, which is the strong\n  posture expected of an email-deliverability vendor.\n- >-\n  No RFC 9116 security.txt is served on any host, and no vulnerability\n  disclosure program or trust center was found — see\n  well-known/debounce-well-known.yml.\ndomains:\n- domain: debounce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: debounce.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/security/debounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Validation
- Email Verification
- Deliverability
- Disposable Email Detection
- MX Records
- Bulk Email Validation
- Data Enrichment
- Syntax Validation
- Reverse Email Lookup
- Logo API
---
