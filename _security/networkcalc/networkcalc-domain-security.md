---
api_specs:
- filename: networkcalc-binary-converter-api-openapi.yml
  format: yaml
  label: NetworkCalc Binary Converter API
  slug: networkcalc-binary-converter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-binary-converter-api-openapi.yml
- filename: networkcalc-dns-api-openapi.yml
  format: yaml
  label: NetworkCalc DNS API
  slug: networkcalc-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-dns-api-openapi.yml
- filename: networkcalc-encoder-api-openapi.yml
  format: yaml
  label: NetworkCalc Encoder API
  slug: networkcalc-encoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-encoder-api-openapi.yml
- filename: networkcalc-security-api-openapi.yml
  format: yaml
  label: NetworkCalc Security API
  slug: networkcalc-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-security-api-openapi.yml
- filename: networkcalc-subnet-calculator-api-openapi.yml
  format: yaml
  label: NetworkCalc Subnet Calculator API
  slug: networkcalc-subnet-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/openapi/networkcalc-subnet-calculator-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: networkcalc.com
  spf: true
hosts:
- cert_expires: Aug  2 04:40:43 2026 GMT
  host: networkcalc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Networkcalc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetworkCalc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: NetworkCalc
provider_slug: networkcalc
slug: networkcalc-domain-security
source_filename: networkcalc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: networkcalc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 04:40:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: networkcalc.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/networkcalc/refs/heads/main/security/networkcalc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Networking
- DNS
- Security
- Subnetting
- Domains
- Calculator
---
