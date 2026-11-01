---
api_specs:
- filename: geocode-farm-openapi-generated.yml
  format: yaml
  label: Geocode.Farm API
  slug: geocode-farm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocode-farm/openapi/_ae-authored/geocode-farm-openapi-generated.yml
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geocodefarm.com
  spf: true
hosts:
- cert_expires: Jan 26 08:58:30 2027 GMT
  host: geocodefarm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geocode Farm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocode.Farm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Geocode.Farm
provider_slug: geocode-farm
slug: geocode-farm-domain-security
source_filename: geocode-farm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geocodefarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 08:58:30 2027 GMT\n  hsts: false\ndomains:\n- domain: geocodefarm.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/geocode-farm/security/geocode-farm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- API
- Location
- Data
- Service
---
