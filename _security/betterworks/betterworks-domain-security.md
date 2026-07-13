---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: betterworks.com
  spf: true
hosts:
- cert_expires: Sep 25 19:25:30 2026 GMT
  host: www.betterworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 15:59:03 2026 GMT
  host: developers.betterworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:31:03 2026 GMT
  host: app.betterworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betterworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterWorks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BetterWorks
provider_slug: betterworks
slug: betterworks-domain-security
source_filename: betterworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betterworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.betterworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.betterworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:31:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: betterworks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterworks/refs/heads/main/security/betterworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- OKR
- Performance Management
- Goals
- Employee Data
- HR
- Enterprise
- Feedback
- Check-ins
- Continuous Performance
- People Analytics
---
