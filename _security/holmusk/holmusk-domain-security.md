---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: holmusk.com
  spf: true
hosts:
- cert_expires: Oct  3 17:27:59 2026 GMT
  host: www.holmusk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holmusk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holmusk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Holmusk
provider_slug: holmusk
slug: holmusk-domain-security
source_filename: holmusk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.holmusk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:27:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: holmusk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holmusk/refs/heads/main/security/holmusk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Real-World Evidence
- Behavioral Health
- Mental Health
- Neuropsychiatry
- Clinical Data
- Data Analytics
- Life Sciences
- HIPAA
---
