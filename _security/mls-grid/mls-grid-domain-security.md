---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mlsgrid.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.mlsgrid.com
  hsts: false
  https: true
  note: Probed manually — every anonymous request returns HTTP 401 (or HTTP 400 "COMPRESSION REQUIRED" without Accept-Encoding gzip), so the automated prober skipped it. Server header nginx/1.30.3, HTTP/2, no Strict-Transport-Security response header.
  tls_version: TLSv1.2
- cert_expires: Sep 29 04:32:43 2026 GMT
  host: www.mlsgrid.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: app.mlsgrid.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 04:03:47 2026 GMT
  host: docs.mlsgrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mls Grid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MLS Grid, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MLS Grid
provider_slug: mls-grid
slug: mls-grid-domain-security
source_filename: mls-grid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mlsgrid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Probed manually — every anonymous request returns HTTP 401 (or HTTP 400 \"COMPRESSION REQUIRED\"\n    without Accept-Encoding gzip), so the automated prober skipped it. Server header nginx/1.30.3,\n    HTTP/2, no Strict-Transport-Security response header.\n- host: www.mlsgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.mlsgrid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: docs.mlsgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mlsgrid.com\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mls-grid/refs/heads/main/security/mls-grid-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Real Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- OData
- Data Licensing
---
