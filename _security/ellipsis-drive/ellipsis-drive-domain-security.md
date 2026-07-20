---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ellipsis-drive.com
  spf: true
hosts:
- cert_expires: Sep 27 19:13:48 2026 GMT
  host: ellipsis-drive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 08:25:47 2026 GMT
  host: docs.ellipsis-drive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:16:58 2026 GMT
  host: api.ellipsis-drive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ellipsis Drive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ellipsis Drive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ellipsis Drive
provider_slug: ellipsis-drive
slug: ellipsis-drive-domain-security
source_filename: ellipsis-drive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ellipsis-drive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ellipsis-drive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:25:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ellipsis-drive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:16:58 2026 GMT\n  hsts: false\ndomains:\n- domain: ellipsis-drive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellipsis-drive/refs/heads/main/security/ellipsis-drive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Geospatial
- Spatial Data
- GIS
- Mapping
- Data Management
- Raster
- Vector
- OGC
- Cloud Storage
- Remote Sensing
---
