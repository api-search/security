---
api_specs:
- filename: latlng-work-geocoding-api-openapi.yml
  format: yaml
  label: latlng-work Geocoding API
  slug: latlng-work-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latlng-work/openapi/latlng-work-geocoding-api-openapi.yml
- filename: latlng-work-places-api-openapi.yml
  format: yaml
  label: latlng-work Places API
  slug: latlng-work-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latlng-work/openapi/latlng-work-places-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: latlng.work
  spf: true
hosts:
- cert_expires: Jan 25 15:57:14 2027 GMT
  host: latlng.work
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latlng Work Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for latlng-work, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: latlng-work
provider_slug: latlng-work
slug: latlng-work-domain-security
source_filename: latlng-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latlng.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 15:57:14 2027 GMT\n  hsts: false\ndomains:\n- domain: latlng.work\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/latlng-work/security/latlng-work-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geocoding
- Mapping
- API
- Location
---
