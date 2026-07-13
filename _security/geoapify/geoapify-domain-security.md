---
api_specs:
- filename: geoapify-forward-geocoding-api-openapi.yml
  format: yaml
  label: Forward Geocoding API
  slug: forward-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoapify/refs/heads/main/openapi/geoapify-forward-geocoding-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geoapify.com
  spf: true
hosts:
- cert_expires: Sep 12 20:25:35 2026 GMT
  host: www.geoapify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 20:25:35 2026 GMT
  host: apidocs.geoapify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 20:25:35 2026 GMT
  host: maps.geoapify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geoapify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geoapify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geoapify
provider_slug: geoapify
slug: geoapify-domain-security
source_filename: geoapify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geoapify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:25:35 2026 GMT\n  hsts: false\n- host: apidocs.geoapify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:25:35 2026 GMT\n  hsts: false\n- host: maps.geoapify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:25:35 2026 GMT\n  hsts: null\ndomains:\n- domain: geoapify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoapify/refs/heads/main/security/geoapify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Geospatial
- Location
- Maps
---
