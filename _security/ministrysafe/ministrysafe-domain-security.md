---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ministrysafe.com
  spf: true
hosts:
- cert_expires: Feb  9 05:20:28 2027 GMT
  host: ministrysafe.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MinistrySafe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MinistrySafe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MinistrySafe
provider_slug: ministrysafe
slug: ministrysafe-domain-security
source_filename: ministrysafe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ministrysafe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 05:20:28 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ministrysafe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ministrysafe/security/ministrysafe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Child Safety
- Education
- Non-Profit
- Training
- Risk Management
---
