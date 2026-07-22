---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tortus.ai
  spf: false
hosts:
- cert_expires: Sep 10 15:55:55 2026 GMT
  host: tortus.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tortus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tortus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Tortus
provider_slug: tortus
slug: tortus-domain-security
source_filename: tortus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tortus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:55:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tortus.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tortus/refs/heads/main/security/tortus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Ambient Clinical Documentation
- Medical Scribe
- Speech to Text
- EHR Integration
- NHS
- Embed SDK
---
