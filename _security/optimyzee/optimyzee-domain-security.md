---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: optimyzee.com
  spf: true
hosts:
- cert_expires: Oct 14 18:49:35 2026 GMT
  host: optimyzee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Optimyzee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optimyzee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Optimyzee
provider_slug: optimyzee
slug: optimyzee-domain-security
source_filename: optimyzee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optimyzee.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 18:49:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: optimyzee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimyzee/refs/heads/main/security/optimyzee-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Advertising
- Google Ads
- PPC
- Marketing
- Automation
- Artificial Intelligence
- SaaS
---
