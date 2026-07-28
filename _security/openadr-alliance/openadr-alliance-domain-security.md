---
api_specs:
- filename: openadr-3-1-1-openapi.yaml
  format: yaml
  label: OpenADR 3 API
  slug: openadr-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openadr-alliance/refs/heads/main/openapi/openadr-3-1-1-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openadr.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
hosts:
- cert_expires: Oct  2 19:56:56 2026 GMT
  host: www.openadr.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: virtserver.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openadr Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenADR Alliance, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenADR Alliance
provider_slug: openadr-alliance
slug: openadr-alliance-domain-security
source_filename: openadr-alliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openadr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: virtserver.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: openadr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openadr-alliance/refs/heads/main/security/openadr-alliance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Demand Response
- Grid
- DER
- OpenADR
- Standards
- Smart Grid
- EV Charging
- Certification
---
