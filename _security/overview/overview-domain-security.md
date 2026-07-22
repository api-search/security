---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: overview.ai
  spf: true
hosts:
- cert_expires: Aug 21 15:50:49 2026 GMT
  host: overview.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overview Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overview, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Overview
provider_slug: overview
slug: overview-domain-security
source_filename: overview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: overview.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 15:50:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: overview.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overview/refs/heads/main/security/overview-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Machine Vision
- Manufacturing
- Quality Control
- Computer Vision
- Edge AI
- Industrial Automation
---
