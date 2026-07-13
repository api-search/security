---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: klippa.com
  spf: true
hosts:
- cert_expires: Sep 11 19:39:43 2026 GMT
  host: www.klippa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: custom-ocr.klippa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: api.klippa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klippa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klippa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Klippa
provider_slug: klippa
slug: klippa-domain-security
source_filename: klippa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klippa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:39:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: custom-ocr.klippa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.klippa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: klippa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klippa/refs/heads/main/security/klippa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Document AI
- IDP
- OCR
- Verification
- GDPR
- EU
---
