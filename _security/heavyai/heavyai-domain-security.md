---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heavy.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nvidia.com
  spf: true
hosts:
- host: www.heavy.ai
  https: false
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: docs.nvidia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heavyai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HEAVY.AI, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HEAVY.AI
provider_slug: heavyai
slug: heavyai-domain-security
source_filename: heavyai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heavy.ai\n  https: false\n- host: docs.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heavy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: nvidia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heavyai/refs/heads/main/security/heavyai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Analytics
- Database
- GPU
- SQL
- Geospatial
- Data Visualization
- Data Science
- Business Intelligence
---
