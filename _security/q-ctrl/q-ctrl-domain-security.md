---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: q-ctrl.com
  spf: true
hosts:
- cert_expires: Oct 15 01:53:35 2026 GMT
  host: q-ctrl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Q Ctrl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Q Ctrl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Q Ctrl
provider_slug: q-ctrl
slug: q-ctrl-domain-security
source_filename: q-ctrl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: q-ctrl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:53:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: q-ctrl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/q-ctrl/refs/heads/main/security/q-ctrl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quantum Computing
- Quantum Control
- Quantum Sensing
- Error Suppression
- Developer Tools
- SDK
- GraphQL API
---
