---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stackyard.ai
  spf: true
hosts:
- cert_expires: Jan 16 16:21:54 2027 GMT
  host: stackyard.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stackyard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackYard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StackYard
provider_slug: stackyard
slug: stackyard-domain-security
source_filename: stackyard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackyard.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 16:21:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stackyard.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackyard/refs/heads/main/security/stackyard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Marketplace
- Directory
- Reviews
- AI Tools
---
