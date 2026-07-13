---
api_specs:
- filename: schema
  format: yaml
  label: World Time API
  slug: world-time-api
  spec_type: OpenAPI
  url: https://timeapi.world/schema
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
