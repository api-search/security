---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: csx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shipcsx.com
  spf: true
hosts:
- cert_expires: Aug 25 18:19:26 2026 GMT
  host: www.csx.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 21:26:27 2026 GMT
  host: shipcsx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Csx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CSX Corporation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CSX Corporation
provider_slug: csx
slug: csx-domain-security
source_filename: csx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.csx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:19:26 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: shipcsx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 21:26:27 2026 GMT\n  hsts: null\ndomains:\n- domain: csx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shipcsx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csx/refs/heads/main/security/csx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Class I Railroad
- Freight
- Intermodal
- Logistics
- Rail
- Transportation
- Fortune 500
---
