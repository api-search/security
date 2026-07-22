---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nanovms.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: nanovms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nanovms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NanoVMs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NanoVMs
provider_slug: nanovms
slug: nanovms-domain-security
source_filename: nanovms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanovms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nanovms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanovms/refs/heads/main/security/nanovms-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Unikernels
- Virtualization
- Cloud Infrastructure
- DevOps
- Open Source
- Developer Tools
- CLI
---
