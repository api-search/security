---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matterfact.com
  spf: true
hosts:
- cert_expires: Feb  8 19:49:14 2027 GMT
  host: matterfact.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Matterfact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matterfact, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matterfact
provider_slug: matterfact-com
slug: matterfact-com-domain-security
source_filename: matterfact-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matterfact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 19:49:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: matterfact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/matterfact-com/security/matterfact-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Artificial Intelligence
- Data
- Enterprise
- Investment
---
