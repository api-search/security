---
api_specs:
- filename: openfeature-openapi.yaml
  format: yaml
  label: OpenFeature Evaluation API
  slug: openfeature-spec
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfeature/refs/heads/main/openapi/openfeature-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openfeature.dev
  spf: true
hosts:
- cert_expires: Sep 19 21:15:27 2026 GMT
  host: openfeature.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openfeature Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenFeature, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenFeature
provider_slug: openfeature
slug: openfeature-domain-security
source_filename: openfeature-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openfeature.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:15:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openfeature.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfeature/refs/heads/main/security/openfeature-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Feature Flags
- Feature Management
- Incubating
- SDKs
- Specification
---
