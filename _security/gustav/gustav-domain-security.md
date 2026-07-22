---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gustav.app
  spf: true
hosts:
- cert_expires: Aug 26 01:11:56 2026 GMT
  host: www.gustav.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gustav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gustav, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gustav
provider_slug: gustav
slug: gustav-domain-security
source_filename: gustav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gustav.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:11:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gustav.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gustav/refs/heads/main/security/gustav-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Staffing
- Vendor Management
- VMS
- Recruiting
- Marketplace
- Contingent Workforce
- HR Tech
- ATS Integration
---
