---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: augmate.io
  spf: true
hosts:
- cert_expires: Nov 30 12:44:15 2026 GMT
  host: augmate.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Augmate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Augmate
provider_slug: augmate
slug: augmate-domain-security
source_filename: augmate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: augmate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 12:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: augmate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmate/refs/heads/main/security/augmate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IoT
- Wearables
- Device Management
- Enterprise
---
