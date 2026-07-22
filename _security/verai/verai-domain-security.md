---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ver-ai.com
  spf: true
hosts:
- cert_expires: Oct  8 14:17:12 2026 GMT
  host: ver-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VerAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VerAI
provider_slug: verai
slug: verai-domain-security
source_filename: verai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ver-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:17:12 2026 GMT\n  hsts: false\ndomains:\n- domain: ver-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verai/refs/heads/main/security/verai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Mining
- Mineral Exploration
- Geoscience
- Critical Minerals
- Geospatial
---
