---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coverhound.com
  spf: true
hosts:
- cert_expires: Oct 14 13:46:05 2026 GMT
  host: coverhound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coverhound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoverHound, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CoverHound
provider_slug: coverhound
slug: coverhound-domain-security
source_filename: coverhound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coverhound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:46:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coverhound.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coverhound/refs/heads/main/security/coverhound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- InsurTech
- Insurance Marketplace
- Comparison Shopping
- Small Business Insurance
---
