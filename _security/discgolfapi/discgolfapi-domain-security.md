---
api_specs:
- filename: discgolfapi-openapi.yml
  format: yaml
  label: DiscGolfAPI REST API
  slug: discgolfapi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discgolfapi/refs/heads/main/openapi/discgolfapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: discgolfapi.com
  spf: true
hosts:
- cert_expires: Aug 31 03:23:34 2026 GMT
  host: discgolfapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 03:23:34 2026 GMT
  host: io.discgolfapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discgolfapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DiscGolfAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DiscGolfAPI
provider_slug: discgolfapi
slug: discgolfapi-domain-security
source_filename: discgolfapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: discgolfapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: io.discgolfapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:23:34 2026 GMT\n  hsts: false\ndomains:\n- domain: discgolfapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discgolfapi/refs/heads/main/security/discgolfapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Disc Golf
- Sports
- Courses
- Open Data
- Recreation
---
