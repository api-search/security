---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humanarchive.ai
  spf: false
hosts:
- cert_expires: Oct  8 21:44:14 2026 GMT
  host: www.humanarchive.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Human Archive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Human Archive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Human Archive
provider_slug: human-archive
slug: human-archive-domain-security
source_filename: human-archive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humanarchive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: humanarchive.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-archive/refs/heads/main/security/human-archive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Artificial Intelligence
- Machine Learning
- Datasets
- Robotics
- Multimodal
- Data Labeling
---
