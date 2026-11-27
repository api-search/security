---
api_specs:
- filename: luviner-com-account-api-openapi.yml
  format: yaml
  label: Luviner Account API
  slug: luviner-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-account-api-openapi.yml
- filename: luviner-com-catalog-api-openapi.yml
  format: yaml
  label: Luviner Catalog API
  slug: luviner-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-catalog-api-openapi.yml
- filename: luviner-com-inference-api-openapi.yml
  format: yaml
  label: Luviner Inference API
  slug: luviner-com-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-inference-api-openapi.yml
- filename: luviner-com-models-api-openapi.yml
  format: yaml
  label: Luviner Models API
  slug: luviner-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-models-api-openapi.yml
- filename: luviner-com-synthetic-data-api-openapi.yml
  format: yaml
  label: Luviner Synthetic Data API
  slug: luviner-com-synthetic-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-synthetic-data-api-openapi.yml
- filename: luviner-com-training-api-openapi.yml
  format: yaml
  label: Luviner Training API
  slug: luviner-com-training-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luviner-com/openapi/luviner-com-training-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: luviner.com
  spf: true
hosts:
- cert_expires: Jan 11 08:02:03 2027 GMT
  host: luviner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Luviner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luviner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Luviner
provider_slug: luviner-com
slug: luviner-com-domain-security
source_filename: luviner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luviner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 08:02:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: luviner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/luviner-com/security/luviner-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Bot Protection
- Self-Hosted
- Web Security
- Italy
---
