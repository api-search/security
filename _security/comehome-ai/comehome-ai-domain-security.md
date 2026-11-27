---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: comehome.ai
  spf: true
hosts:
- cert_expires: Jan 26 08:25:18 2027 GMT
  host: www.comehome.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ComeHome.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComeHome.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ComeHome.ai
provider_slug: comehome-ai
slug: comehome-ai-domain-security
source_filename: comehome-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comehome.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 08:25:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: comehome.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/comehome-ai/security/comehome-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Moving
- Moving Cost Estimates
- Virtual Survey
- Computer Vision
- Lead Scoring
- Artificial Intelligence
- MCP
---
