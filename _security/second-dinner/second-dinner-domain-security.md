---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seconddinner.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.seconddinner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Second Dinner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Second Dinner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Second Dinner
provider_slug: second-dinner
slug: second-dinner-domain-security
source_filename: second-dinner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seconddinner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seconddinner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/second-dinner/refs/heads/main/security/second-dinner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video Games
- Game Development
- Gaming
- Entertainment
- Mobile Games
- Card Games
- Unity
---
