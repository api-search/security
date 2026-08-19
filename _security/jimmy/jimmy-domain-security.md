---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jimmy-energy.eu
  spf: true
hosts:
- cert_expires: Sep 30 23:15:13 2026 GMT
  host: www.jimmy-energy.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jimmy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jimmy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jimmy
provider_slug: jimmy
slug: jimmy-domain-security
source_filename: jimmy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jimmy-energy.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jimmy-energy.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jimmy/refs/heads/main/security/jimmy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate Tech
- Energy
- Nuclear
- Small Modular Reactor
- Industrial Heat
- Decarbonization
- Deep Tech
- Manufacturing
- France
---
