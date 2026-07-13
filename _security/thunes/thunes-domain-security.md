---
api_specs:
- filename: thunes-openapi.yml
  format: yaml
  label: Thunes Money Transfer API
  slug: thunes-money-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thunes/refs/heads/main/openapi/thunes-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:infrastructure+sslalerts@thunes.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thunes.com
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.thunes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: docs.thunes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.thunes.com
  https: false
kind: domain-security
layout: security
method: probed
name: Thunes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thunes, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thunes
provider_slug: thunes
slug: thunes-domain-security
source_filename: thunes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thunes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\n- host: docs.thunes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thunes.com\n  https: false\ndomains:\n- domain: thunes.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:infrastructure+sslalerts@thunes.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thunes/refs/heads/main/security/thunes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Cross-Border
- Payments
- FX
- Mobile Money
---
