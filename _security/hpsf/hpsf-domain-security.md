---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hpsf.io
  spf: true
hosts:
- cert_expires: Nov 25 05:52:28 2026 GMT
  host: www.hpsf.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hpsf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for High Performance Software Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: High Performance Software Foundation
provider_slug: hpsf
slug: hpsf-domain-security
source_filename: hpsf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hpsf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 05:52:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: hpsf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hpsf/refs/heads/main/security/hpsf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HPC
- Linux Foundation
- Open Source
- Scientific Computing
- Foundations
- Supercomputing
- Open Governance
- Event
- Conferences
- Research Computing
- Non-Profit
- Content
---
