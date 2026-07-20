---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carto.com
  spf: true
hosts:
- cert_expires: Sep  9 15:36:52 2026 GMT
  host: docs.carto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:38:07 2026 GMT
  host: gcp-us-east1.api.carto.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cartodb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CARTO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CARTO
provider_slug: cartodb
slug: cartodb-domain-security
source_filename: cartodb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.carto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gcp-us-east1.api.carto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:38:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: carto.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartodb/refs/heads/main/security/cartodb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Location Intelligence
- Geospatial
- Maps
- Spatial Analytics
- Data Warehouse
- GIS
- Agents
---
