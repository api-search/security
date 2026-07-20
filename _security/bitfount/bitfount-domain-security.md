---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitfount.com
  spf: true
hosts:
- cert_expires: Aug 21 23:00:28 2026 GMT
  host: bitfount.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitfount Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitfount, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bitfount
provider_slug: bitfount
slug: bitfount-domain-security
source_filename: bitfount-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitfount.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:00:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitfount.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfount/refs/heads/main/security/bitfount-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Federated Learning
- Machine Learning
- Data Science
- Privacy
- Artificial Intelligence
- Healthcare
- Python SDK
- Data Collaboration
---
