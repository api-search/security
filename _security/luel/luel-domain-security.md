---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: luel.ai
  spf: true
hosts:
- cert_expires: Aug 24 19:32:10 2026 GMT
  host: www.luel.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Luel
provider_slug: luel
slug: luel-domain-security
source_filename: luel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.luel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:32:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: luel.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luel/refs/heads/main/security/luel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Machine Learning
- Training Data
- Data Marketplace
- Multimodal
- Video
- Audio
- Data Licensing
---
