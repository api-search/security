---
api_specs:
- filename: lago-openapi.yml
  format: yaml
  label: Lago API
  slug: lago-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getlago.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: getlago.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:40:11 2026 GMT
  host: api.getlago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 20:11:05 2026 GMT
  host: api.eu.getlago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lago, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lago
provider_slug: lago
slug: lago-domain-security
source_filename: lago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getlago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.getlago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:40:11 2026 GMT\n  hsts: null\n- host: api.eu.getlago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 20:11:05 2026 GMT\n  hsts: null\ndomains:\n- domain: getlago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/security/lago-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Billing
- Metering
- Open Source
- Usage-Based
---
