---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: craon.ai
  spf: true
hosts:
- cert_expires: Aug 26 02:25:18 2026 GMT
  host: craon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Craon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Craon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Craon
provider_slug: craon
slug: craon-domain-security
source_filename: craon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: craon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craon/refs/heads/main/security/craon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video Editing
- Artificial Intelligence
- Video
- Content Creation
- Media
- Creative Tools
---
