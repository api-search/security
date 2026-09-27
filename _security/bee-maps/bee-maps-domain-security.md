---
api_specs:
- filename: bee-maps-account-api-openapi.yml
  format: yaml
  label: Bee Maps Account API
  slug: bee-maps-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-account-api-openapi.yml
- filename: bee-maps-ai-events-api-openapi.yml
  format: yaml
  label: Bee Maps AI Events API
  slug: bee-maps-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-ai-events-api-openapi.yml
- filename: bee-maps-bursts-api-openapi.yml
  format: yaml
  label: Bee Maps Bursts API
  slug: bee-maps-bursts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-bursts-api-openapi.yml
- filename: bee-maps-devices-api-openapi.yml
  format: yaml
  label: Bee Maps Devices API
  slug: bee-maps-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-devices-api-openapi.yml
- filename: bee-maps-imagery-api-openapi.yml
  format: yaml
  label: Bee Maps Imagery API
  slug: bee-maps-imagery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-imagery-api-openapi.yml
- filename: bee-maps-map-features-api-openapi.yml
  format: yaml
  label: Bee Maps Map Features API
  slug: bee-maps-map-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-map-features-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaqprivatemarket.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: beemaps.com
  spf: true
hosts:
- cert_expires: Dec 21 07:53:45 2026 GMT
  host: www.nasdaqprivatemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 11:58:07 2026 GMT
  host: beemaps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bee Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bee Maps, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bee Maps
provider_slug: bee-maps
slug: bee-maps-domain-security
source_filename: bee-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaqprivatemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: beemaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 11:58:07 2026 GMT\n  hsts: false\ndomains:\n- domain: nasdaqprivatemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: beemaps.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/security/bee-maps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mapping
- GIS
- Location
- Data
---
