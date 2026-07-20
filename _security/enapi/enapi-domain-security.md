---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: enapi.com
  spf: true
hosts:
- cert_expires: Oct 15 12:35:58 2026 GMT
  host: enapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:19:28 2026 GMT
  host: docs.enapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 10:15:08 2026 GMT
  host: roaming.enapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enapi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Enapi
provider_slug: enapi
slug: enapi-domain-security
source_filename: enapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:35:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.enapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:19:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: roaming.enapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:15:08 2026 GMT\n  hsts: null\ndomains:\n- domain: enapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enapi/refs/heads/main/security/enapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EV Charging
- OCPI
- Roaming
- E-Mobility
- Charge Point Operator
- eMSP
- Electric Vehicle
- CDR Clearing
- Interoperability
- Hub
---
