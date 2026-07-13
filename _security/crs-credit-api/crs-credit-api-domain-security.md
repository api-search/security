---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crscreditapi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: redoc.ly
  spf: true
hosts:
- cert_expires: Aug 16 12:17:57 2026 GMT
  host: crscreditapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: crscreditapi.redoc.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: api-sandbox.stitchcredit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Crs Credit Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRS Credit API, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CRS Credit API
provider_slug: crs-credit-api
slug: crs-credit-api-domain-security
source_filename: crs-credit-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crscreditapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 12:17:57 2026 GMT\n  hsts: false\n- host: crscreditapi.redoc.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.stitchcredit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: crscreditapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: redoc.ly\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crs-credit-api/refs/heads/main/security/crs-credit-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Credit
- Consumer Credit
- Business Credit
- Identity
- Fraud
- Data
---
