---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: breezm.com
  spf: false
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: breezm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breezm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breezm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Breezm
provider_slug: breezm
slug: breezm-domain-security
source_filename: breezm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breezm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: breezm.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breezm/refs/heads/main/security/breezm-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Eyewear
- Custom Glasses
- 3D Scanning
- Sustainable
---
