---
api_specs:
- filename: gammaflip-io-data-api-openapi.yml
  format: yaml
  label: GammaFlip.io Data API
  slug: gammaflip-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gammaflip-io/openapi/gammaflip-io-data-api-openapi.yml
- filename: gammaflip-io-discovery-api-openapi.yml
  format: yaml
  label: GammaFlip.io Discovery API
  slug: gammaflip-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gammaflip-io/openapi/gammaflip-io-discovery-api-openapi.yml
- filename: gammaflip-io-history-api-openapi.yml
  format: yaml
  label: GammaFlip.io History API
  slug: gammaflip-io-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gammaflip-io/openapi/gammaflip-io-history-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gammaflip.io
  spf: true
hosts:
- cert_expires: Jan 16 08:18:50 2027 GMT
  host: gammaflip.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GammaFlip.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GammaFlip.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GammaFlip.io
provider_slug: gammaflip-io
slug: gammaflip-io-domain-security
source_filename: gammaflip-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gammaflip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 08:18:50 2027 GMT\n  hsts: false\ndomains:\n- domain: gammaflip.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gammaflip-io/security/gammaflip-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Cryptocurrency
- Market Data
- Trading
---
