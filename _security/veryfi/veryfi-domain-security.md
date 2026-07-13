---
api_specs:
- filename: veryfi-ocr-openapi.yml
  format: yaml
  label: Veryfi OCR API
  slug: ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-ocr-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@veryfi.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: veryfi.com
  spf: true
hosts:
- cert_expires: Aug 21 01:30:10 2026 GMT
  host: www.veryfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 01:30:10 2026 GMT
  host: docs.veryfi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 01:30:10 2026 GMT
  host: api.veryfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veryfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veryfi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Veryfi
provider_slug: veryfi
slug: veryfi-domain-security
source_filename: veryfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veryfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:30:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.veryfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:30:10 2026 GMT\n  hsts: false\n- host: api.veryfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:30:10 2026 GMT\n  hsts: null\ndomains:\n- domain: veryfi.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@veryfi.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/security/veryfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Document Processing
- Finance
- Invoices
- OCR
- Receipts
- Tax Forms
---
