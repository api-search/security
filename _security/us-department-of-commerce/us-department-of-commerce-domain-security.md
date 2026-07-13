---
api_specs:
- filename: commerce-gov-api-openapi.yml
  format: yaml
  label: Commerce.gov API
  slug: commercegov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-department-of-commerce/refs/heads/main/openapi/commerce-gov-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: commerce.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: census.gov
  spf: true
hosts:
- cert_expires: Aug 24 01:39:28 2026 GMT
  host: www.commerce.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:56:12 2026 GMT
  host: www.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: apps.bea.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Department Of Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Department of Commerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Department of Commerce
provider_slug: us-department-of-commerce
slug: us-department-of-commerce-domain-security
source_filename: us-department-of-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commerce.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:39:28 2026 GMT\n  hsts: null\n- host: www.census.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apps.bea.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commerce.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: census.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-department-of-commerce/refs/heads/main/security/us-department-of-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commerce
- Federal Government
- Open Data
- Trade
- Economic Data
- Climate
- Standards
---
