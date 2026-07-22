---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: houserx.com
  spf: true
hosts:
- cert_expires: Sep 28 00:30:27 2026 GMT
  host: www.houserx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: House Rx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for House Rx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: House Rx
provider_slug: house-rx
slug: house-rx-domain-security
source_filename: house-rx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.houserx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: houserx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/house-rx/refs/heads/main/security/house-rx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Specialty Pharmacy
- Pharmacy
- Medically Integrated Dispensing
- Prior Authorization
- Health Technology
- EHR Integration
- Patient Care
---
