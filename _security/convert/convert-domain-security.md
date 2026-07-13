---
api_specs:
- filename: convert-openapi.yml
  format: yaml
  label: Convert Experiences REST API v2
  slug: convert-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convert/refs/heads/main/openapi/convert-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convert.com
  spf: false
hosts:
- cert_expires: Aug 20 17:33:33 2026 GMT
  host: www.convert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.convert.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: apidev.convert.com
  https: false
kind: domain-security
layout: security
method: probed
name: Convert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convert, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Convert
provider_slug: convert
slug: convert-domain-security
source_filename: convert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.convert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:33:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.convert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: apidev.convert.com\n  https: false\ndomains:\n- domain: convert.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convert/refs/heads/main/security/convert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Experimentation
- AB Testing
- Conversion Optimization
- Personalization
- Analytics
---
