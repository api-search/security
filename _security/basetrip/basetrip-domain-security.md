---
api_specs:
- filename: basetrip-api-openapi.yml
  format: yaml
  label: Basetrip API
  slug: basetrip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/openapi/basetrip-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thebasetrip.com
  spf: true
hosts:
- cert_expires: Sep 15 01:12:35 2026 GMT
  host: www.thebasetrip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 00:02:42 2026 GMT
  host: api.thebasetrip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basetrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basetrip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Basetrip
provider_slug: basetrip
slug: basetrip-domain-security
source_filename: basetrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thebasetrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:12:35 2026 GMT\n  hsts: false\n- host: api.thebasetrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:02:42 2026 GMT\n  hsts: false\ndomains:\n- domain: thebasetrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/security/basetrip-domain-security.yml
summary_line: TLSv1.3
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
---
