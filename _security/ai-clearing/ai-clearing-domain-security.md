---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aiclearing.com
  spf: true
hosts:
- cert_expires: Nov  1 02:26:21 2026 GMT
  host: www.aiclearing.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ai Clearing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Clearing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AI Clearing
provider_slug: ai-clearing
slug: ai-clearing-domain-security
source_filename: ai-clearing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aiclearing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 02:26:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aiclearing.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-clearing/refs/heads/main/security/ai-clearing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Construction
- Construction Technology
- Artificial Intelligence
- Computer-Vision
- Drones
- Geospatial
- Digital Twin
- Progress Tracking
- Quality Control
- Renewable Energy
- Infrastructure
---
