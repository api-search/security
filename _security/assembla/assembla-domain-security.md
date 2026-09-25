---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: assembla.com
  spf: true
hosts:
- cert_expires: Feb 25 11:50:13 2027 GMT
  host: www.assembla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Assembla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assembla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Assembla
provider_slug: assembla
slug: assembla-domain-security
source_filename: assembla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.assembla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 11:50:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: assembla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assembla/refs/heads/main/security/assembla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Version Control
- Cloud Hosting
- DevOps
- Project Management
- Security
---
