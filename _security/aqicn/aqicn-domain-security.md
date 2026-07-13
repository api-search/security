---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aqicn.org
  spf: true
hosts:
- cert_expires: Aug  8 05:59:26 2026 GMT
  host: aqicn.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aqicn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AQICN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AQICN
provider_slug: aqicn
slug: aqicn-domain-security
source_filename: aqicn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aqicn.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  8 05:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: aqicn.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqicn/refs/heads/main/security/aqicn-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Weather
- Public APIs
---
