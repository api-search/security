---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: winnebagoind.com
  spf: true
hosts:
- cert_expires: Oct  8 06:31:46 2026 GMT
  host: www.winnebagoind.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Winnebago Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Winnebago Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Winnebago Industries
provider_slug: winnebago-industries
slug: winnebago-industries-domain-security
source_filename: winnebago-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.winnebagoind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:31:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: winnebagoind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/winnebago-industries/refs/heads/main/security/winnebago-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recreational Vehicles
- Manufacturing
- Outdoor
- Consumer Products
---
