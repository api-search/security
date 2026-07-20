---
api_specs:
- filename: hydrosat-stac-openapi.json
  format: json
  label: Hydrosat Discovery STAC API
  slug: hydrosat-discovery-stac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrosat/refs/heads/main/openapi/hydrosat-stac-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hydrosat.com
  spf: true
hosts:
- cert_expires: Sep 26 09:25:33 2026 GMT
  host: hydrosat.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hydrosat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydrosat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hydrosat
provider_slug: hydrosat
slug: hydrosat-domain-security
source_filename: hydrosat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydrosat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 09:25:33 2026 GMT\n  hsts: false\ndomains:\n- domain: hydrosat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrosat/refs/heads/main/security/hydrosat-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Satellite Imagery
- Thermal Infrared
- Geospatial
- Earth Observation
- Remote Sensing
- STAC
- Agriculture
- Water Management
- Data
---
