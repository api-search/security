---
api_specs:
- filename: wakatime-api-v1-openapi.yml
  format: yaml
  label: WakaTime API v1
  slug: wakatime-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/openapi/wakatime-api-v1-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wakatime.com
  spf: true
hosts:
- cert_expires: Sep 10 07:07:57 2026 GMT
  host: wakatime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 07:03:12 2026 GMT
  host: api.wakatime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wakatime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WakaTime, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WakaTime
provider_slug: wakatime
slug: wakatime-domain-security
source_filename: wakatime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wakatime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wakatime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wakatime.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wakatime/refs/heads/main/security/wakatime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Productivity
- Developer Tools
- Time Tracking
- Coding Analytics
- Leaderboards
- IDE Plugins
- Open Source
- Public APIs
---
