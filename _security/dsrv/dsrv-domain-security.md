---
api_specs:
- filename: dsrv-ethereum-api-openapi.yml
  format: yaml
  label: Dsrv Ethereum API
  slug: dsrv-ethereum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsrv/openapi/dsrv-ethereum-api-openapi.yml
- filename: dsrv-health-api-openapi.yml
  format: yaml
  label: Dsrv Health API
  slug: dsrv-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsrv/openapi/dsrv-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dsrv.com
  spf: false
hosts:
- cert_expires: Jan  4 23:45:02 2027 GMT
  host: www.dsrv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dsrv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dsrv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dsrv
provider_slug: dsrv
slug: dsrv-domain-security
source_filename: dsrv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dsrv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:45:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dsrv.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dsrv/security/dsrv-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Blockchain
- Infrastructure
- Staking
- Web3
---
