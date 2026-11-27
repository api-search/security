---
api_specs:
- filename: maxoperf-com-academy-openapi-generated.yml
  format: yaml
  label: MaxoPerf Overview API
  slug: academy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-academy-openapi-generated.yml
- filename: maxoperf-com-core-openapi-generated.yml
  format: yaml
  label: MaxoPerf core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-core-openapi-generated.yml
- filename: maxoperf-com-dependencies-openapi-generated.yml
  format: yaml
  label: MaxoPerf Overview API
  slug: dependencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-dependencies-openapi-generated.yml
- filename: maxoperf-com-how-to-openapi-generated.yml
  format: yaml
  label: MaxoPerf how to API
  slug: how-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-how-to-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maxoperf.com
  spf: false
hosts:
- cert_expires: Jan 29 11:13:35 2027 GMT
  host: maxoperf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MaxoPerf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaxoPerf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MaxoPerf
provider_slug: maxoperf-com
slug: maxoperf-com-domain-security
source_filename: maxoperf-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maxoperf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 11:13:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maxoperf.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maxoperf-com/security/maxoperf-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Performance Testing
- Load Testing
- Cloud
---
