---
api_specs:
- filename: normapi-com-openapi.yml
  format: yaml
  label: NormAPI REST API
  slug: normapi-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normapi-com/openapi/normapi-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: normapi.com
  spf: true
hosts:
- cert_expires: Jan  1 21:45:09 2027 GMT
  host: normapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Normapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NormAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NormAPI
provider_slug: normapi-com
slug: normapi-com-domain-security
source_filename: normapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: normapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 21:45:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: normapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/normapi-com/security/normapi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- e-invoicing
- XRechnung
- ZUGFeRD
- Germany
---
