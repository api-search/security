---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thecommons.earth
  spf: true
hosts:
- cert_expires: Sep 10 00:18:18 2026 GMT
  host: www.thecommons.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Commons
provider_slug: commons
slug: commons-domain-security
source_filename: commons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecommons.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 00:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thecommons.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commons/refs/heads/main/security/commons-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- Carbon Footprint
- Carbon Offsets
- Personal Finance
- Consumer Fintech
- Sustainability
- Mobile Application
- Consumer Application
- California
---
