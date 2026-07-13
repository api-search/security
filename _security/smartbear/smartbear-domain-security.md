---
api_specs:
- filename: smartbear-swaggerhub-openapi.yml
  format: yaml
  label: SwaggerHub API
  slug: swaggerhub
  spec_type: OpenAPI
  url: https://openapi/smartbear-swaggerhub-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartbear.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swagger.io
  spf: true
hosts:
- cert_expires: Sep 15 04:10:42 2026 GMT
  host: smartbear.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 16:46:01 2026 GMT
  host: swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: pactflow.io
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Smartbear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartBear, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SmartBear
provider_slug: smartbear
slug: smartbear-domain-security
source_filename: smartbear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartbear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:10:42 2026 GMT\n  hsts: false\n- host: swagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:46:01 2026 GMT\n  hsts: false\n- host: pactflow.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\ndomains:\n- domain: smartbear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swagger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/security/smartbear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Documentation
- API Testing
- Contract Testing
- Governance
- Monitoring
- Platform
---
