---
api_specs:
- filename: api-fiddle-api-fiddle-openapi.yml
  format: yaml
  label: API-Fiddle
  slug: api-fiddle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/openapi/api-fiddle-api-fiddle-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: api-fiddle.com
  spf: false
hosts:
- cert_expires: Sep 16 09:51:38 2026 GMT
  host: api-fiddle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 17:15:41 2026 GMT
  host: api.api-fiddle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Fiddle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API-Fiddle, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: API-Fiddle
provider_slug: api-fiddle
slug: api-fiddle-domain-security
source_filename: api-fiddle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-fiddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 09:51:38 2026 GMT\n  hsts: false\n- host: api.api-fiddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:15:41 2026 GMT\n  hsts: false\ndomains:\n- domain: api-fiddle.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/security/api-fiddle-domain-security.yml
summary_line: TLSv1.3
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
---
