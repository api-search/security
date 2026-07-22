---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hybird.ai
  spf: true
hosts:
- cert_expires: Sep 22 19:18:13 2026 GMT
  host: www.hybird.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hybird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HyBird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HyBird
provider_slug: hybird
slug: hybird-domain-security
source_filename: hybird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hybird.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:18:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hybird.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hybird/refs/heads/main/security/hybird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Twin
- Industrial Operating System
- Asset Management
- Maintenance Management
- Inspection
- Environment Health and Safety
- Reality Capture
- Heavy Industry
---
