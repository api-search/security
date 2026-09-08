---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adgager.com
  spf: true
hosts:
- cert_expires: Nov 14 09:16:25 2026 GMT
  host: www.adgager.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 06:40:52 2026 GMT
  host: dash.adgager.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 11:00:41 2026 GMT
  host: api.adgager.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Adgager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adgager, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adgager
provider_slug: adgager
slug: adgager-domain-security
source_filename: adgager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adgager.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 09:16:25 2026 GMT\n  hsts: false\n- host: dash.adgager.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 06:40:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adgager.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 11:00:41 2026 GMT\n  hsts: false\ndomains:\n- domain: adgager.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adgager/refs/heads/main/security/adgager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Research
- Consumer Insights
- Survey
- Advertising
- Advertising Effectiveness
- Brand Measurement
- Panel
- GraphQL
- Turkey
---
