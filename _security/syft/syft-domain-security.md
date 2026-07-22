---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: syftapp.com
  spf: true
hosts:
- cert_expires: Sep 14 13:15:43 2026 GMT
  host: syftapp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Syft
provider_slug: syft
slug: syft-domain-security
source_filename: syft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syftapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:15:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: syftapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syft/refs/heads/main/security/syft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Other
- Staffing
- Recruitment
- Hospitality
- Workforce
- Marketplace
- Gig Economy
---
