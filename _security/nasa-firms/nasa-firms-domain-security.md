---
api_specs:
- filename: nasa-firms-openapi.yml
  format: yaml
  label: FIRMS Area Fire Detections API
  slug: area-fire-detections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-firms/refs/heads/main/openapi/nasa-firms-openapi.yml
- filename: nasa-firms-openapi.yml
  format: yaml
  label: FIRMS KML Fire Footprints API
  slug: kml-fire-footprints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-firms/refs/heads/main/openapi/nasa-firms-openapi.yml
- filename: nasa-firms-openapi.yml
  format: yaml
  label: FIRMS Data Availability API
  slug: data-availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-firms/refs/heads/main/openapi/nasa-firms-openapi.yml
- filename: nasa-firms-openapi.yml
  format: yaml
  label: FIRMS Missing Data API
  slug: missing-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-firms/refs/heads/main/openapi/nasa-firms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
hosts:
- cert_expires: Sep  5 04:17:50 2026 GMT
  host: firms.modaps.eosdis.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nasa Firms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA FIRMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NASA FIRMS
provider_slug: nasa-firms
slug: nasa-firms-domain-security
source_filename: nasa-firms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firms.modaps.eosdis.nasa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 04:17:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-firms/refs/heads/main/security/nasa-firms-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- NASA
- Fire Detection
- Satellite
- MODIS
- VIIRS
- Remote Sensing
- Open Data
- Environmental
- Geospatial
- Science
---
