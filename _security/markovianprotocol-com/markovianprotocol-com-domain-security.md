---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: markovianprotocol.com
  spf: true
hosts:
- cert_expires: Jan 12 11:09:53 2027 GMT
  host: markovianprotocol.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Markovian Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markovian Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Markovian Protocol
provider_slug: markovianprotocol-com
slug: markovianprotocol-com-domain-security
source_filename: markovianprotocol-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markovianprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 11:09:53 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: markovianprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/markovianprotocol-com/security/markovianprotocol-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Transparency
- Data
- Open Source
- Research
---
