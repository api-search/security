---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bloomtech.com
  spf: true
hosts:
- cert_expires: Oct 16 14:12:47 2026 GMT
  host: www.bloomtech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bloomtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BloomTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BloomTech
provider_slug: bloomtech
slug: bloomtech-domain-security
source_filename: bloomtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bloomtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomtech/refs/heads/main/security/bloomtech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coding Bootcamp
- Developer Training
- AI‑Integrated Learning
- Career Support
- Deferred Tuition
---
