---
api_specs:
- filename: score-openapi.yml
  format: yaml
  label: Score Workload Specification API
  slug: score-workload-specification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/score-openapi.yml
- filename: cloud-native-application-bundle-openapi.yml
  format: yaml
  label: Cloud Native Application Bundle API
  slug: cloud-native-application-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/cloud-native-application-bundle-openapi.yml
- filename: open-component-model-openapi.yml
  format: yaml
  label: Open Component Model API
  slug: open-component-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/open-component-model-openapi.yml
- filename: open-resource-discovery-openapi.yml
  format: yaml
  label: Open Resource Discovery API
  slug: open-resource-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/open-resource-discovery-openapi.yml
- filename: radius-openapi.yml
  format: yaml
  label: Radius Application Platform API
  slug: radius-application-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/radius-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: score.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cnab.io
  spf: false
hosts:
- cert_expires: Aug 15 00:07:20 2026 GMT
  host: score.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.score.dev
  https: false
- cert_expires: Sep 11 02:31:27 2026 GMT
  host: cnab.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Application Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Application Research, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Application Research
provider_slug: application-research
slug: application-research-domain-security
source_filename: application-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: score.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 00:07:20 2026 GMT\n  hsts: false\n- host: api.score.dev\n  https: false\n- host: cnab.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:31:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: score.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cnab.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/security/application-research-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Application Dependencies
- Cloud Native
- Integration
- Research
- Specifications
- Workload Specifications
---
