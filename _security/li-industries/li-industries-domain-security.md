---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: li-ind.com
  spf: true
hosts:
- cert_expires: Sep 28 17:31:13 2026 GMT
  host: www.li-ind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Li Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Li Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Li Industries
provider_slug: li-industries
slug: li-industries-domain-security
source_filename: li-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.li-ind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:31:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: li-ind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/li-industries/refs/heads/main/security/li-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Battery Recycling
- Lithium-Ion Batteries
- Battery Materials
- Cathode Active Material
- Circular Economy
- Clean Energy
- Advanced Manufacturing
---
