---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: daivin.tech
  spf: true
hosts:
- cert_expires: Sep  4 03:54:36 2026 GMT
  host: www.daivin.tech
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daivin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daivin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Daivin
provider_slug: daivin
slug: daivin-domain-security
source_filename: daivin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daivin.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:54:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: daivin.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daivin/refs/heads/main/security/daivin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Deep Tech
- Hardware
- Diving
- Electrolysis
- Oxygen Generation
- Life Support
- Y Combinator
- San Francisco
---
