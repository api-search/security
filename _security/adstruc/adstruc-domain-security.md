---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adstruc.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: adstruc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adstruc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADstruc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ADstruc
provider_slug: adstruc
slug: adstruc-domain-security
source_filename: adstruc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adstruc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: adstruc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adstruc/refs/heads/main/security/adstruc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Out-of-Home
- OOH
- AdTech
- Digital Out-of-Home
- Media Buying
- Marketing
---
