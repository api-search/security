---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dapdip.com
  spf: false
hosts:
- cert_expires: Dec 31 08:04:50 2026 GMT
  host: dapdip.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dapdip Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DapDip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: DapDip
provider_slug: dapdip-com
slug: dapdip-com-domain-security
source_filename: dapdip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dapdip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 08:04:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dapdip.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dapdip-com/security/dapdip-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- YouTube
- CreatorGrowth
- Analytics
- Artificial Intelligence
- Platform
---
