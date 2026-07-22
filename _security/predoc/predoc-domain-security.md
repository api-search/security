---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: predoc.ai
  spf: true
hosts:
- cert_expires: Sep 24 14:20:18 2026 GMT
  host: www.predoc.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 19:20:02 2026 GMT
  host: docs.predoc.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: partner-sandbox.predoc.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Predoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Predoc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Predoc
provider_slug: predoc
slug: predoc-domain-security
source_filename: predoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.predoc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.predoc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-sandbox.predoc.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: predoc.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/security/predoc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Records
- Health Information Exchange
- FHIR
- Clinical Data
- AI
- Interoperability
- EHR Integration
- Webhooks
- Clinical Research
---
