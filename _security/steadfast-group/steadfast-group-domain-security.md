---
api_specs:
- filename: steadfast-group-address-api-openapi.yml
  format: yaml
  label: Steadfast Group Address API
  slug: steadfast-group-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-address-api-openapi.yml
- filename: steadfast-group-risk-api-openapi.yml
  format: yaml
  label: Steadfast Group Risk API
  slug: steadfast-group-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-risk-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steadfast.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steadfastagencies.com.au
  spf: true
hosts:
- cert_expires: Jan  8 10:58:47 2027 GMT
  host: www.steadfast.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 03:46:16 2026 GMT
  host: steadfastagencies.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  7 00:11:38 2027 GMT
  host: www.steadfastlife.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Steadfast Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steadfast Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Steadfast Group
provider_slug: steadfast-group
slug: steadfast-group-domain-security
source_filename: steadfast-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.steadfast.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 10:58:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: steadfastagencies.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 03:46:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.steadfastlife.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 00:11:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: steadfast.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: steadfastagencies.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/security/steadfast-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Brokerage
- Insurance Broker Network
- General Insurance
- Property and Casualty
- Underwriting Agency
- Agency Management
- ACORD
- New Zealand
---
