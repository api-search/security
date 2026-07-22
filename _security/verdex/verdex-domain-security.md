---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verdexai.com
  spf: true
hosts:
- cert_expires: Sep 15 16:18:28 2026 GMT
  host: www.verdexai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verdex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verdex
provider_slug: verdex
slug: verdex-domain-security
source_filename: verdex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verdexai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: verdexai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdex/refs/heads/main/security/verdex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Clinical Documentation
- Artificial Intelligence
- Voice AI
- Electronic Health Records
- HIPAA
- Medical Scribe
---
