---
api_specs:
- filename: sunrise-atelier-ip-api-openapi.yml
  format: yaml
  label: Sunrise Atelier Ip API
  slug: sunrise-atelier-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sunrise-atelier/refs/heads/main/openapi/sunrise-atelier-ip-api-openapi.yml
- filename: sunrise-atelier-timezone-api-openapi.yml
  format: yaml
  label: Sunrise Atelier Timezone API
  slug: sunrise-atelier-timezone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sunrise-atelier/refs/heads/main/openapi/sunrise-atelier-timezone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sunrise.am
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: time.now
  spf: false
hosts:
- cert_expires: Oct  9 12:05:32 2026 GMT
  host: sunrise.am
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:02:51 2026 GMT
  host: time.now
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunrise Atelier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunrise Atelier, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sunrise Atelier
provider_slug: sunrise-atelier
slug: sunrise-atelier-domain-security
source_filename: sunrise-atelier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunrise.am\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:05:32 2026 GMT\n  hsts: false\n- host: time.now\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:02:51 2026 GMT\n  hsts: false\ndomains:\n- domain: sunrise.am\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: time.now\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunrise-atelier/refs/heads/main/security/sunrise-atelier-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Time
- Timezone
- Astronomy
- Geolocation
- Sunrise
- Sunset
- Developer API
---
