---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ausgrid.com.au
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.ausgrid.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: services.ausgrid.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: idoportal.ausgrid.com.au
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ausgrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ausgrid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ausgrid
provider_slug: ausgrid
slug: ausgrid-domain-security
source_filename: ausgrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ausgrid.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: services.ausgrid.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: idoportal.ausgrid.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552001\ndomains:\n- domain: ausgrid.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ausgrid/refs/heads/main/security/ausgrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- Consumer Data Right
- Solar
- DER
- Outages
---
