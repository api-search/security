---
api_specs:
- filename: soldcomps-io-account-api-openapi.yml
  format: yaml
  label: SoldComps.io Account API
  slug: soldcomps-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldcomps-io/openapi/soldcomps-io-account-api-openapi.yml
- filename: soldcomps-io-sold-comps-api-openapi.yml
  format: yaml
  label: SoldComps.io Sold comps API
  slug: soldcomps-io-sold-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldcomps-io/openapi/soldcomps-io-sold-comps-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soldcomps.io
  spf: false
hosts:
- cert_expires: Jan 21 02:00:02 2027 GMT
  host: www.soldcomps.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SoldComps.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoldComps.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: SoldComps.io
provider_slug: soldcomps-io
slug: soldcomps-io-domain-security
source_filename: soldcomps-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soldcomps.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 02:00:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: soldcomps.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/soldcomps-io/security/soldcomps-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eBay
- Pricing
- Data
- Marketplace
---
