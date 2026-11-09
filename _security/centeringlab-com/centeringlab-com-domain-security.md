---
api_specs:
- filename: centeringlab-com-grade-api-openapi.yml
  format: yaml
  label: Centering Lab Grade API
  slug: centeringlab-com-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-grade-api-openapi.yml
- filename: centeringlab-com-health-api-openapi.yml
  format: yaml
  label: Centering Lab Health API
  slug: centeringlab-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-health-api-openapi.yml
- filename: centeringlab-com-measure-api-openapi.yml
  format: yaml
  label: Centering Lab Measure API
  slug: centeringlab-com-measure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-measure-api-openapi.yml
- filename: centeringlab-com-openapi-json-api-openapi.yml
  format: yaml
  label: Centering Lab Openapi.json API
  slug: centeringlab-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-openapi-json-api-openapi.yml
- filename: centeringlab-com-standards-api-openapi.yml
  format: yaml
  label: Centering Lab Standards API
  slug: centeringlab-com-standards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-standards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: centeringlab.com
  spf: true
hosts:
- cert_expires: Dec 30 15:40:08 2026 GMT
  host: centeringlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centeringlab Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centering Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Centering Lab
provider_slug: centeringlab-com
slug: centeringlab-com-domain-security
source_filename: centeringlab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centeringlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 15:40:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: centeringlab.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/centeringlab-com/security/centeringlab-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Cards
- Centering
- Collectors
- Web App
---
