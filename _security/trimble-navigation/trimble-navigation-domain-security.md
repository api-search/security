---
api_specs:
- filename: trimble-mobile-manager-openapi.yml
  format: yaml
  label: Trimble Mobile Manager API
  slug: trimble-mobile-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/openapi/trimble-mobile-manager-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trimble.com
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
kind: domain-security
layout: security
method: probed
name: Trimble Navigation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trimble Navigation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trimble Navigation
provider_slug: trimble-navigation
slug: trimble-navigation-domain-security
source_filename: trimble-navigation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:53:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trimble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trimble-navigation/refs/heads/main/security/trimble-navigation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPS
- GNSS
- Positioning
- Navigation
- Surveying
- Geospatial
- Construction
- Fortune 1000
---
