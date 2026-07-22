---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aspinity.com
  spf: true
hosts:
- cert_expires: Oct  7 19:04:15 2026 GMT
  host: aspinity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aspinity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aspinity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aspinity
provider_slug: aspinity
slug: aspinity-domain-security
source_filename: aspinity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aspinity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:04:15 2026 GMT\n  hsts: false\ndomains:\n- domain: aspinity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspinity/refs/heads/main/security/aspinity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Machine Learning
- Edge AI
- IoT
- Analog Computing
- Hardware
---
