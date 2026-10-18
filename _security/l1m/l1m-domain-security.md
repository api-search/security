---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: l1m.io
  spf: false
hosts:
- cert_expires: Jan  9 02:43:22 2027 GMT
  host: l1m.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: L1M Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for l1m.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: l1m.io
provider_slug: l1m
slug: l1m-domain-security
source_filename: l1m-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: l1m.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 02:43:22 2027 GMT\n  hsts: false\ndomains:\n- domain: l1m.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/l1m/refs/heads/main/security/l1m-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data Extraction
- LLM
- API
- Open Source
---
