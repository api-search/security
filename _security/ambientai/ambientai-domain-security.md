---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ambient.ai
  spf: true
hosts:
- cert_expires: Aug 28 17:49:08 2026 GMT
  host: www.ambient.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambientai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambient.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ambient.ai
provider_slug: ambientai
slug: ambientai-domain-security
source_filename: ambientai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambient.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:49:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ambient.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambientai/refs/heads/main/security/ambientai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Security
- Computer Vision
- Artificial Intelligence
- Video Analytics
- Access Control
- Threat Detection
- Enterprise Security
- Agentic AI
---
