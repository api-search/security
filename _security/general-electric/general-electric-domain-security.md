---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ge.com
  spf: false
hosts:
- cert_expires: Sep 17 06:28:18 2026 GMT
  host: www.ge.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Electric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: General Electric
provider_slug: general-electric
slug: general-electric-domain-security
source_filename: general-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:28:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ge.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-electric/refs/heads/main/security/general-electric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Aviation
- Energy
- Manufacturing
- Fortune 500
---
