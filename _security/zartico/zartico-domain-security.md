---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zartico.com
  spf: true
hosts:
- cert_expires: Nov  7 00:31:48 2026 GMT
  host: www.zartico.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 01:57:04 2026 GMT
  host: geoserver.zartico.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 00:23:18 2026 GMT
  host: login.zartico.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Zartico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zartico, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zartico
provider_slug: zartico
slug: zartico-domain-security
source_filename: zartico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zartico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: geoserver.zartico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 01:57:04 2026 GMT\n  hsts: null\n- host: login.zartico.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 00:23:18 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: zartico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zartico/refs/heads/main/security/zartico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Tourism
- Destination Marketing
- Location Intelligence
- Geospatial
- Analytics
- Data
- Business Intelligence
- OGC
---
