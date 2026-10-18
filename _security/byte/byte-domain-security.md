---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bytetechnology.co
  spf: true
hosts:
- cert_expires: Nov 29 19:00:11 2026 GMT
  host: bytetechnology.co
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Byte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Byte
provider_slug: byte
slug: byte-domain-security
source_filename: byte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bytetechnology.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 19:00:11 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: bytetechnology.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byte/refs/heads/main/security/byte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food-Service
- Retail
- Technology
- Software-as-a-Service
---
