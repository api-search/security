---
api_specs:
- filename: openstreetmap-capabilities-api-openapi.yml
  format: yaml
  label: OpenStreetMap Capabilities API
  slug: openstreetmap-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-capabilities-api-openapi.yml
- filename: openstreetmap-changesets-api-openapi.yml
  format: yaml
  label: OpenStreetMap Changesets API
  slug: openstreetmap-changesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-changesets-api-openapi.yml
- filename: openstreetmap-map-data-api-openapi.yml
  format: yaml
  label: OpenStreetMap Map Data API
  slug: openstreetmap-map-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-map-data-api-openapi.yml
- filename: openstreetmap-nodes-api-openapi.yml
  format: yaml
  label: OpenStreetMap Nodes API
  slug: openstreetmap-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-nodes-api-openapi.yml
- filename: openstreetmap-notes-api-openapi.yml
  format: yaml
  label: OpenStreetMap Notes API
  slug: openstreetmap-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-notes-api-openapi.yml
- filename: openstreetmap-relations-api-openapi.yml
  format: yaml
  label: OpenStreetMap Relations API
  slug: openstreetmap-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-relations-api-openapi.yml
- filename: openstreetmap-users-api-openapi.yml
  format: yaml
  label: OpenStreetMap Users API
  slug: openstreetmap-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-users-api-openapi.yml
- filename: openstreetmap-ways-api-openapi.yml
  format: yaml
  label: OpenStreetMap Ways API
  slug: openstreetmap-ways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-ways-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openstreetmap.org
  spf: true
hosts:
- cert_expires: Sep  1 21:25:37 2026 GMT
  host: www.openstreetmap.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 18:15:51 2026 GMT
  host: wiki.openstreetmap.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 21:25:37 2026 GMT
  host: api.openstreetmap.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openstreetmap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenStreetMap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OpenStreetMap
provider_slug: openstreetmap
slug: openstreetmap-domain-security
source_filename: openstreetmap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openstreetmap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:25:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wiki.openstreetmap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openstreetmap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:25:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openstreetmap.org\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/security/openstreetmap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Geospatial
- Mapping
- Open Data
- Geocoding
- Editing
---
