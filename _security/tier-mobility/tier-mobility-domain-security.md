---
api_specs:
- filename: tier-mobility-discovery-api-openapi.yml
  format: yaml
  label: TIER Discovery API
  slug: tier-mobility-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-discovery-api-openapi.yml
- filename: tier-mobility-stations-api-openapi.yml
  format: yaml
  label: TIER Stations API
  slug: tier-mobility-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-stations-api-openapi.yml
- filename: tier-mobility-system-api-openapi.yml
  format: yaml
  label: TIER System API
  slug: tier-mobility-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-system-api-openapi.yml
- filename: tier-mobility-vehicles-api-openapi.yml
  format: yaml
  label: TIER Vehicles API
  slug: tier-mobility-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-vehicles-api-openapi.yml
- filename: tier-mobility-zones-api-openapi.yml
  format: yaml
  label: TIER Zones API
  slug: tier-mobility-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-zones-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ridedott.com
  spf: true
hosts:
- cert_expires: Sep  8 07:04:44 2026 GMT
  host: ridedott.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 06:18:25 2026 GMT
  host: gbfs.api.ridedott.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tier Mobility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIER, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TIER
provider_slug: tier-mobility
slug: tier-mobility-domain-security
source_filename: tier-mobility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ridedott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:04:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gbfs.api.ridedott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 06:18:25 2026 GMT\n  hsts: null\ndomains:\n- domain: ridedott.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/security/tier-mobility-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mobility
- Micromobility
- Shared Mobility
- E-Scooter
- E-Bike
- Transportation
- Smart Cities
- MaaS
- GBFS
- Open Data
- Europe
- Real-Time
---
