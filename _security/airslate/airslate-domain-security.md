---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airslate.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signnow.com
  spf: true
hosts:
- cert_expires: Sep  4 18:29:10 2026 GMT
  host: www.airslate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:01:05 2026 GMT
  host: docs.signnow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 17:54:47 2026 GMT
  host: api.signnow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airslate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for airSlate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: airSlate
provider_slug: airslate
slug: airslate-domain-security
source_filename: airslate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airslate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 18:29:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.signnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:01:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.signnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:54:47 2026 GMT\n  hsts: null\ndomains:\n- domain: airslate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: signnow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/security/airslate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Automation
- eSignature
- Workflow
- PDF
- No-Code
- AI
---
