---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: heldly.io
  spf: true
hosts:
- cert_expires: Feb  4 14:42:49 2027 GMT
  host: heldly.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heldly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heldly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Heldly
provider_slug: heldly-io
slug: heldly-io-domain-security
source_filename: heldly-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heldly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 14:42:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heldly.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/heldly-io/security/heldly-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Productivity
- To-Do List
- Free
---
