---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: velaura.ai
  spf: true
hosts:
- cert_expires: Sep 25 23:29:31 2026 GMT
  host: velaura.ai
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auradine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auradine (Velaura AI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Auradine (Velaura AI)
provider_slug: auradine
slug: auradine-domain-security
source_filename: auradine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velaura.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:29:31 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: velaura.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auradine/refs/heads/main/security/auradine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- AI Infrastructure
- Low Power AI Compute
- Blockchain
- Bitcoin Mining
- Data Center
- Silicon
- Edge Computing
- Hardware
---
