---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eliyan.com
  spf: true
hosts:
- cert_expires: Oct  7 14:39:18 2026 GMT
  host: eliyan.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eliyan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eliyan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eliyan
provider_slug: eliyan
slug: eliyan-domain-security
source_filename: eliyan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eliyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:39:18 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: eliyan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliyan/refs/heads/main/security/eliyan-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductors
- Chiplets
- Silicon IP
- Interconnect
- SerDes
- Artificial Intelligence
- High Performance Computing
- Data-Center
- Hardware
---
