---
api_specs:
- filename: federal-communications-commission-datasets-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Datasets API
  slug: federal-communications-commission-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-datasets-api-openapi.yml
- filename: federal-communications-commission-filings-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Filings API
  slug: federal-communications-commission-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-filings-api-openapi.yml
- filename: federal-communications-commission-pirate-radio-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Pirate Radio API
  slug: federal-communications-commission-pirate-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-pirate-radio-api-openapi.yml
- filename: federal-communications-commission-proceedings-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Proceedings API
  slug: federal-communications-commission-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-proceedings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fcc.gov
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: www.fcc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 17:20:54 2026 GMT
  host: publicapi.fcc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 02:52:22 2027 GMT
  host: opendata.fcc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Federal Communications Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Communications Commission, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Communications Commission
provider_slug: federal-communications-commission
slug: federal-communications-commission-domain-security
source_filename: federal-communications-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fcc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: null\n- host: publicapi.fcc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:20:54 2026 GMT\n  hsts: null\n- host: opendata.fcc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 02:52:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fcc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/security/federal-communications-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Communications
- Federal Government
- Open Data
---
