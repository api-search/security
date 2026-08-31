---
api_specs:
- filename: telia-listgeographicsite-api-openapi.yml
  format: yaml
  label: Telia Company List Geographic Site API
  slug: telia-listgeographicsite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/openapi/telia-listgeographicsite-api-openapi.yml
- filename: telia-retrievegeographicsite-api-openapi.yml
  format: yaml
  label: Telia Company Retrieve Geographic Site API
  slug: telia-retrievegeographicsite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/openapi/telia-retrievegeographicsite-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teliacompany.com
  spf: true
hosts:
- cert_expires: Sep 29 10:14:19 2026 GMT
  host: www.teliacompany.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 15 09:31:57 2026 GMT
  host: lso.teliacompany.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 15 12:00:23 2026 GMT
  host: api-garden.teliacompany.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Telia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telia Company, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Telia Company
provider_slug: telia
slug: telia-domain-security
source_filename: telia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teliacompany.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 10:14:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: lso.teliacompany.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 09:31:57 2026 GMT\n  hsts: null\n- host: api-garden.teliacompany.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 12:00:23 2026 GMT\n  hsts: null\ndomains:\n- domain: teliacompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/security/telia-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Telecommunications
- Sweden
- Nordics
- Baltics
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- Messaging
- SMS
- SMPP
- IoT
- 5G
- Broadband
- Identity Verification
- BSS
- OSS
- TM Forum
- MEF
- Standards
---
