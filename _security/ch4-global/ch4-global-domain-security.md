---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ch4global.com
  spf: true
hosts:
- cert_expires: Aug 29 06:03:52 2026 GMT
  host: ch4global.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ch4 Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ch4 Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ch4 Global
provider_slug: ch4-global
slug: ch4-global-domain-security
source_filename: ch4-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ch4global.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:03:52 2026 GMT\n  hsts: false\ndomains:\n- domain: ch4global.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ch4-global/refs/heads/main/security/ch4-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Methane
- Agriculture
- Livestock
- Sustainability
- Seaweed
- Carbon
---
