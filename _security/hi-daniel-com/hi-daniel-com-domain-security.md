---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hi-daniel.com
  spf: true
hosts:
- cert_expires: Jan  9 16:30:45 2027 GMT
  host: hi-daniel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daniel Liu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daniel Liu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daniel Liu
provider_slug: hi-daniel-com
slug: hi-daniel-com-domain-security
source_filename: hi-daniel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hi-daniel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 16:30:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hi-daniel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hi-daniel-com/security/hi-daniel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Artificial Intelligence
- Growth
- B2B
- Developers
---
