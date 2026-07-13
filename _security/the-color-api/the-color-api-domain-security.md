---
api_specs:
- filename: the-color-api-openapi.yml
  format: yaml
  label: The Color API
  slug: the-color-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-color-api/refs/heads/main/openapi/the-color-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thecolorapi.com
  spf: true
hosts:
- cert_expires: Aug 12 01:38:54 2026 GMT
  host: www.thecolorapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Color Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Color API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: The Color API
provider_slug: the-color-api
slug: the-color-api-domain-security
source_filename: the-color-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecolorapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 01:38:54 2026 GMT\n  hsts: false\ndomains:\n- domain: thecolorapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-color-api/refs/heads/main/security/the-color-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Colors
- Design
- Utilities
---
