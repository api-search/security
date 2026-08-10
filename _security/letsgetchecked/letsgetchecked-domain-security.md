---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: letsgetchecked.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.letsgetchecked.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: docs.letsgetchecked.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Letsgetchecked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LetsGetChecked, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LetsGetChecked
provider_slug: letsgetchecked
slug: letsgetchecked-domain-security
source_filename: letsgetchecked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.letsgetchecked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.letsgetchecked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: letsgetchecked.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letsgetchecked/refs/heads/main/security/letsgetchecked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Laboratory
- Telehealth
- Medical Testing
- Pharmacy
- Orders
- Results
- Webhooks
- HL7
- LOINC
---
