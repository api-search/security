---
api_specs:
- filename: time-now-openapi-generated.yml
  format: yaml
  label: Time.now API
  slug: time-now-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/time-now/refs/heads/main/openapi/_ae-authored/time-now-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: time.now
  spf: false
hosts:
- cert_expires: Jan 10 15:02:51 2027 GMT
  host: time.now
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Time Now Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Time.now, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Time.now
provider_slug: time-now
slug: time-now-domain-security
source_filename: time-now-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: time.now\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 15:02:51 2027 GMT\n  hsts: false\ndomains:\n- domain: time.now\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/time-now/refs/heads/main/security/time-now-domain-security.yml
summary_line: TLSv1.3
tags:
- World Time API
- Developer Tools
- IoT
- Web Applications
- Timezones
- Geolocation
---
