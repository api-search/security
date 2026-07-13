---
api_specs:
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Authentication API
  slug: eight-sleep-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep User API
  slug: eight-sleep-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Device API
  slug: eight-sleep-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Temperature API
  slug: eight-sleep-temperature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Trends API
  slug: eight-sleep-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Base API
  slug: eight-sleep-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Alarms API
  slug: eight-sleep-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eightsleep.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 8slp.net
  spf: true
hosts:
- cert_expires: Sep 16 02:45:46 2026 GMT
  host: www.eightsleep.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: auth-api.8slp.net
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: client-api.8slp.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eight Sleep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eight Sleep, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eight Sleep
provider_slug: eight-sleep
slug: eight-sleep-domain-security
source_filename: eight-sleep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eightsleep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:45:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: auth-api.8slp.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\n- host: client-api.8slp.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: eightsleep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 8slp.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/security/eight-sleep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sleep
- IoT
- Smart Home
- Wearables
- Health
- Unofficial
---
