---
api_specs:
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Organizations API
  slug: propeller-aero-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Sites API
  slug: propeller-aero-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Surveys API
  slug: propeller-aero-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Workspaces API
  slug: propeller-aero-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Shapes & Widgets API
  slug: propeller-aero-shapes-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Position Monitoring API
  slug: propeller-aero-position-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: propelleraero.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 28 18:39:13 2026 GMT
  host: www.propelleraero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: propelleraero.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.propelleraero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propeller Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propeller Aero, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Propeller Aero
provider_slug: propeller-aero
slug: propeller-aero-domain-security
source_filename: propeller-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propelleraero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:39:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: propelleraero.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.propelleraero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: propelleraero.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/security/propeller-aero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Drone Survey
- Geospatial
- Earthworks
- Construction
- Mining
- Photogrammetry
- Surveying
- Analytics
---
