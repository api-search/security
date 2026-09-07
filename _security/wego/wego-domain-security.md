---
api_specs:
- filename: wego-api-openapi.json
  format: json
  label: Wego API
  slug: wego-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wego.com
  spf: true
hosts:
- cert_expires: Dec  3 07:01:58 2026 GMT
  host: www.wego.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 03:38:14 2026 GMT
  host: docs.wego.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 07:01:58 2026 GMT
  host: api.wego.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Wego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wego, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wego
provider_slug: wego
slug: wego-domain-security
source_filename: wego-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 07:01:58 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.wego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 03:38:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 07:01:58 2026 GMT\n  hsts: null\ndomains:\n- domain: wego.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/security/wego-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Flights
- Hotels
- Metasearch
- Booking
- Agent Native
- Tourism
- Search
---
