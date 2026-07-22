---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: districtcover.com
  spf: true
hosts:
- cert_expires: Oct  5 05:48:13 2026 GMT
  host: districtcover.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: District Cover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for District Cover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: District Cover
provider_slug: district-cover
slug: district-cover-domain-security
source_filename: district-cover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: districtcover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:48:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: districtcover.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/district-cover/refs/heads/main/security/district-cover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Insurtech
- Commercial Insurance
- Underwriting
- Risk Management
- Surplus Lines
- Brokerage
---
