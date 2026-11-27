---
api_specs:
- filename: deeprecall-io-health-api-openapi.yml
  format: yaml
  label: DeepRecall Health API
  slug: deeprecall-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deeprecall-io/openapi/deeprecall-io-health-api-openapi.yml
- filename: deeprecall-io-recalls-api-openapi.yml
  format: yaml
  label: DeepRecall Recalls API
  slug: deeprecall-io-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deeprecall-io/openapi/deeprecall-io-recalls-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deeprecall.io
  spf: false
hosts:
- cert_expires: Jan  3 15:02:55 2027 GMT
  host: deeprecall.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DeepRecall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepRecall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DeepRecall
provider_slug: deeprecall-io
slug: deeprecall-io-domain-security
source_filename: deeprecall-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deeprecall.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 15:02:55 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deeprecall.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/deeprecall-io/security/deeprecall-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Regulatory
- Marketplace
- Compliance
- Intelligence
---
