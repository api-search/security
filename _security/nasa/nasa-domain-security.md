---
api_specs:
- filename: nasa-apod-openapi.yml
  format: yaml
  label: NASA Astronomy Picture of the Day (APOD) API
  slug: apod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-apod-openapi.yml
- filename: nasa-mars-rover-photos-openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-mars-rover-photos-openapi.yml
- filename: nasa-neo-openapi.yml
  format: yaml
  label: NASA NeoWs (Near Earth Object Web Service) API
  slug: neo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-neo-openapi.yml
- filename: nasa-donki-openapi.yml
  format: yaml
  label: NASA DONKI (Space Weather) API
  slug: donki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-donki-openapi.yml
- filename: nasa-epic-openapi.yml
  format: yaml
  label: NASA EPIC (Earth Polychromatic Imaging Camera) API
  slug: epic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-epic-openapi.yml
- filename: nasa-nasa-image-and-video-library-openapi.yml
  format: yaml
  label: NASA Image and Video Library API
  slug: image-and-video-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-nasa-image-and-video-library-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
hosts:
- cert_expires: Aug 31 19:21:07 2026 GMT
  host: api.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 00:21:08 2026 GMT
  host: www.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: images-api.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nasa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NASA
provider_slug: nasa
slug: nasa-domain-security
source_filename: nasa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:21:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: images-api.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/security/nasa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Science
- Space
---
