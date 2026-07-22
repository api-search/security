---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: c-infinity.ai
  spf: true
hosts:
- cert_expires: Sep  4 14:55:23 2026 GMT
  host: c-infinity.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: C Infinity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C-Infinity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: C-Infinity
provider_slug: c-infinity
slug: c-infinity-domain-security
source_filename: c-infinity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: c-infinity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: c-infinity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c-infinity/refs/heads/main/security/c-infinity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Manufacturing
- CAD
- PLM
- Engineering
- Assembly Planning
- Industrial
---
