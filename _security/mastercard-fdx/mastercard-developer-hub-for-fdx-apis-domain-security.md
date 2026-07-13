---
api_specs:
- filename: fdx-authorization-api-openapi.yaml
  format: yaml
  label: Mastercard FDX Authorization API
  slug: authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/fdx-authorization-api-openapi.yaml
- filename: fdx-resource-api-openapi.yaml
  format: yaml
  label: Mastercard FDX Resource API
  slug: resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/fdx-resource-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mastercard.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: developer.mastercard.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mastercard Developer Hub For Fdx Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mastercard Developer Hub for FDX APIs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mastercard Developer Hub for FDX APIs
provider_slug: mastercard-fdx
slug: mastercard-developer-hub-for-fdx-apis-domain-security
source_filename: mastercard-developer-hub-for-fdx-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mastercard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: mastercard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/security/mastercard-developer-hub-for-fdx-apis-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- FDX
- Open Banking
---
