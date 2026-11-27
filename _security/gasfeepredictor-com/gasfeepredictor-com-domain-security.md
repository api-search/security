---
api_specs:
- filename: gasfeepredictor-com-l2-api-openapi.yml
  format: yaml
  label: Gas Fee Predictor L2 API
  slug: gasfeepredictor-com-l2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasfeepredictor-com/openapi/gasfeepredictor-com-l2-api-openapi.yml
- filename: gasfeepredictor-com-mainnet-api-openapi.yml
  format: yaml
  label: Gas Fee Predictor Mainnet API
  slug: gasfeepredictor-com-mainnet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasfeepredictor-com/openapi/gasfeepredictor-com-mainnet-api-openapi.yml
- filename: gasfeepredictor-com-price-api-openapi.yml
  format: yaml
  label: Gas Fee Predictor Price API
  slug: gasfeepredictor-com-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasfeepredictor-com/openapi/gasfeepredictor-com-price-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gasfeepredictor.com
  spf: true
hosts:
- cert_expires: Jan  2 21:14:10 2027 GMT
  host: gasfeepredictor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:43:10 2026 GMT
  host: api.gasfeepredictor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Gas Fee Predictor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gas Fee Predictor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gas Fee Predictor
provider_slug: gasfeepredictor-com
slug: gasfeepredictor-com-domain-security
source_filename: gasfeepredictor-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gasfeepredictor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:14:10 2027 GMT\n  hsts: false\n- host: api.gasfeepredictor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:43:10 2026 GMT\n  hsts: false\ndomains:\n- domain: gasfeepredictor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gasfeepredictor-com/security/gasfeepredictor-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ethereum
- Gas
- Utility
- Free
---
