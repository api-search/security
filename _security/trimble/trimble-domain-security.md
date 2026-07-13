---
api_specs:
- filename: trimble-connect-openapi.yml
  format: yaml
  label: Trimble Connect API
  slug: trimble-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-connect-openapi.yml
- filename: trimble-maps-openapi.yml
  format: yaml
  label: Trimble Maps API
  slug: trimble-maps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-maps-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trimble.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tekla.com
  spf: true
hosts:
- cert_expires: Aug 21 18:53:50 2026 GMT
  host: www.trimble.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:03:44 2026 GMT
  host: developer.trimble.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: developer.tekla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trimble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trimble, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Trimble
provider_slug: trimble
slug: trimble-domain-security
source_filename: trimble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:53:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tekla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trimble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: tekla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/security/trimble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Transportation
- Geospatial
- GPS
- Mapping
- BIM
- Fleet Management
- Collaboration
- Agriculture
---
