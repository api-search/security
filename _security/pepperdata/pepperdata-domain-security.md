---
api_specs:
- filename: pepperdata-rest-api-openapi.yml
  format: yaml
  label: Pepperdata REST API
  slug: pepperdata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pepperdata/refs/heads/main/openapi/pepperdata-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pepperdata.com
  spf: true
hosts:
- cert_expires: Oct 11 08:34:20 2026 GMT
  host: pepperdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pepperdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pepperdata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pepperdata
provider_slug: pepperdata
slug: pepperdata-domain-security
source_filename: pepperdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pepperdata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 08:34:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pepperdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pepperdata/refs/heads/main/security/pepperdata-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Observability
- Monitoring
- Kubernetes
- Big Data
- Cost Optimization
- Metrics
- APM
---
