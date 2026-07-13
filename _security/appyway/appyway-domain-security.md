---
api_specs:
- filename: appyway-availability-realtime-api-openapi.yml
  format: yaml
  label: AppyWay Availability RealTime API
  slug: appyway-availability-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-availability-realtime-api-openapi.yml
- filename: appyway-traffic-data-api-openapi.yml
  format: yaml
  label: AppyWay Traffic Data API
  slug: appyway-traffic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-traffic-data-api-openapi.yml
- filename: appyway-explorer-api-openapi.yml
  format: yaml
  label: AppyWay Explorer API
  slug: appyway-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-explorer-api-openapi.yml
- filename: appyway-platform-api-openapi.yml
  format: yaml
  label: AppyWay Platform API
  slug: appyway-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appyway.com
  spf: true
hosts:
- cert_expires: Sep 15 21:17:04 2026 GMT
  host: docs.appyway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.appyway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appyway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppyWay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppyWay
provider_slug: appyway
slug: appyway-domain-security
source_filename: appyway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.appyway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:17:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.appyway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: appyway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/security/appyway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parking
- Traffic
- Urban Mobility
- Smart Cities
- EV Charging
---
