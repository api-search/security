---
api_specs:
- filename: apinizer-api.yaml
  format: yaml
  label: Apinizer API
  slug: apinizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apinizer/refs/heads/main/openapi/apinizer-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apinizer.com
  spf: true
hosts:
- cert_expires: Aug  4 10:59:48 2026 GMT
  host: apinizer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 06:29:07 2026 GMT
  host: api.apinizer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apinizer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apinizer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apinizer
provider_slug: apinizer
slug: apinizer-domain-security
source_filename: apinizer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apinizer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:59:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apinizer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:29:07 2026 GMT\n  hsts: null\ndomains:\n- domain: apinizer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apinizer/refs/heads/main/security/apinizer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- API Management
- API Monitoring
- API Security
- Policies
---
