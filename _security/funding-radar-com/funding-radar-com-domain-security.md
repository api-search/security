---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: funding-radar.com
  spf: true
hosts:
- cert_expires: Dec 18 00:19:40 2026 GMT
  host: funding-radar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Funding Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Funding Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Funding Radar
provider_slug: funding-radar-com
slug: funding-radar-com-domain-security
source_filename: funding-radar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: funding-radar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 00:19:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: funding-radar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/funding-radar-com/security/funding-radar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Cryptocurrency
- Funding
- Real-Time
- Calculator
---
