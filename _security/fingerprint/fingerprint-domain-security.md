---
api_specs:
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Events API
  slug: fingerprint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Events Search API
  slug: fingerprint-events-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Visitors API
  slug: fingerprint-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Related Visitors API
  slug: fingerprint-related-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Smart Signals API
  slug: fingerprint-smart-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Webhooks
  slug: fingerprint-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
- filename: fingerprint-openapi.yml
  format: yaml
  label: Fingerprint Sealed Results
  slug: fingerprint-sealed-results
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/openapi/fingerprint-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fingerprint.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: fpjs.io
  spf: false
hosts:
- cert_expires: Sep 24 08:36:10 2026 GMT
  host: fingerprint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: dev.fingerprint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.fpjs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fingerprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fingerprint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fingerprint
provider_slug: fingerprint
slug: fingerprint-domain-security
source_filename: fingerprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fingerprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:36:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.fingerprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fpjs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fingerprint.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fpjs.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/security/fingerprint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Device Identification
- Fraud Prevention
- Bot Detection
- Smart Signals
- Identity
---
