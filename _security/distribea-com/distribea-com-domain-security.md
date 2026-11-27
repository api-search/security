---
api_specs:
- filename: distribea-com-account-api-openapi.yml
  format: yaml
  label: Distribea Account API
  slug: distribea-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-account-api-openapi.yml
- filename: distribea-com-catalog-api-openapi.yml
  format: yaml
  label: Distribea Catalog API
  slug: distribea-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-catalog-api-openapi.yml
- filename: distribea-com-generation-api-openapi.yml
  format: yaml
  label: Distribea Generation API
  slug: distribea-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-generation-api-openapi.yml
- filename: distribea-com-models-api-openapi.yml
  format: yaml
  label: Distribea Models API
  slug: distribea-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-models-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: distribea.com
  spf: true
hosts:
- cert_expires: Jan  4 01:50:21 2027 GMT
  host: distribea.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Distribea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distribea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Distribea
provider_slug: distribea-com
slug: distribea-com-domain-security
source_filename: distribea-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distribea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:50:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: distribea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/distribea-com/security/distribea-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Video
- Media
- Software-as-a-Service
- Platform
---
