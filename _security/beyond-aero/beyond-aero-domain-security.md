---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: beyond-aero.com
  spf: true
hosts:
- cert_expires: Sep 23 05:24:53 2026 GMT
  host: www.beyond-aero.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beyond Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beyond Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Beyond Aero
provider_slug: beyond-aero
slug: beyond-aero-domain-security
source_filename: beyond-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beyond-aero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:24:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beyond-aero.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-aero/refs/heads/main/security/beyond-aero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Frontier Tech
- Aviation
- Aerospace
- Hydrogen
- Electric Aircraft
- Sustainable Aviation
- Business Aviation
---
