---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cerevance.com
  spf: true
hosts:
- cert_expires: Oct  3 04:48:43 2026 GMT
  host: cerevance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerevance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerevance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cerevance
provider_slug: cerevance
slug: cerevance-domain-security
source_filename: cerevance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cerevance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:48:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cerevance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerevance/refs/heads/main/security/cerevance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Central Nervous System
- Neuroscience
---
