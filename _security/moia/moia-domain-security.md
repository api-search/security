---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moia.io
  spf: true
hosts:
- cert_expires: Nov 23 20:20:46 2026 GMT
  host: www.moia.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MOIA
provider_slug: moia
slug: moia-domain-security
source_filename: moia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 20:20:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: moia.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moia/refs/heads/main/security/moia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Mobility
- Ridepooling
- Transportation
- Cities
- Software
- Operations
---
