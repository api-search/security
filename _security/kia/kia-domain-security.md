---
api_specs:
- filename: kia-api-api-openapi.yml
  format: yaml
  label: Kia 계정 API
  slug: kia-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kia/refs/heads/main/openapi/kia-api-api-openapi.yml
- filename: kia-default-api-openapi.yml
  format: yaml
  label: Kia 개인정보 제공 동의 및 철회 API
  slug: kia-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kia/refs/heads/main/openapi/kia-default-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kia.com
  spf: true
hosts:
- cert_expires: Apr 15 23:59:59 2027 GMT
  host: www.kia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kia
provider_slug: kia
slug: kia-domain-security
source_filename: kia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kia/refs/heads/main/security/kia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicles
- Vehicle Data
- Authentication
- Company
---
