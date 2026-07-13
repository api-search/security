---
api_specs:
- filename: bls-public-data-api-openapi.yaml
  format: yaml
  label: BLS Public Data API
  slug: bls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-bureau-of-labor-statistics/refs/heads/main/openapi/bls-public-data-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bls.gov
  spf: true
hosts:
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: www.bls.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: api.bls.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: U S Bureau Of Labor Statistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Bureau of Labor Statistics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: U.S. Bureau of Labor Statistics
provider_slug: u-s-bureau-of-labor-statistics
slug: u-s-bureau-of-labor-statistics-domain-security
source_filename: u-s-bureau-of-labor-statistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bls.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: null\n- host: api.bls.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bls.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-bureau-of-labor-statistics/refs/heads/main/security/u-s-bureau-of-labor-statistics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Labor
- Statistics
- Employment
- Economic Data
---
