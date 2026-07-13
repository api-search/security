---
api_specs:
- filename: openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: nasa-mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-mars/main/openapi/openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Nasa Mars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA Mars Rovers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NASA Mars Rovers
provider_slug: nasa-mars
slug: nasa-mars-domain-security
source_filename: nasa-mars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-mars/refs/heads/main/security/nasa-mars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NASA
- Mars
- Rovers
- Photos
- Images
- Space
- Planetary Science
- Open Data
---
