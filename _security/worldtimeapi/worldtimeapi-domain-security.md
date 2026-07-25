---
api_specs:
- filename: worldtimeapi-geo-api-openapi.yml
  format: yaml
  label: World Time API Geo API
  slug: worldtimeapi-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/openapi/worldtimeapi-geo-api-openapi.yml
- filename: worldtimeapi-geo-txt-api-openapi.yml
  format: yaml
  label: World Time API Geo.txt API
  slug: worldtimeapi-geo-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/openapi/worldtimeapi-geo-txt-api-openapi.yml
- filename: worldtimeapi-ip-api-openapi.yml
  format: yaml
  label: World Time API Ip API
  slug: worldtimeapi-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/openapi/worldtimeapi-ip-api-openapi.yml
- filename: worldtimeapi-ip-txt-api-openapi.yml
  format: yaml
  label: World Time API Ip.txt API
  slug: worldtimeapi-ip-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/openapi/worldtimeapi-ip-txt-api-openapi.yml
- filename: worldtimeapi-timezone-api-openapi.yml
  format: yaml
  label: World Time API Timezone API
  slug: worldtimeapi-timezone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/openapi/worldtimeapi-timezone-api-openapi.yml
- filename: worldtimeapi-timezone-txt-api-openapi.yml
  format: yaml
  label: World Time API Timezone.txt API
  slug: worldtimeapi-timezone-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/openapi/worldtimeapi-timezone-txt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: timeapi.world
  spf: false
hosts:
- cert_expires: Oct  5 15:33:09 2026 GMT
  host: timeapi.world
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:33:09 2026 GMT
  host: public.timeapi.world
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worldtimeapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Time API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: World Time API
provider_slug: worldtimeapi
slug: worldtimeapi-domain-security
source_filename: worldtimeapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: timeapi.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:33:09 2026 GMT\n  hsts: false\n- host: public.timeapi.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:33:09 2026 GMT\n  hsts: null\ndomains:\n- domain: timeapi.world\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldtimeapi/refs/heads/main/security/worldtimeapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Time
- Timezone
- World Time
- UTC
- DST
- Daylight Saving Time
- IP Geolocation
- Unix Epoch
---
