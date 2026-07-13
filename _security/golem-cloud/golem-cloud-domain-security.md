---
api_specs:
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Components API
  slug: components
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Workers & Invocation API
  slug: workers-invocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem API Definitions & Deployments API
  slug: api-definitions-deployments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Plugins API
  slug: plugins
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: golem.cloud
  spf: true
hosts:
- cert_expires: Aug 23 22:02:54 2026 GMT
  host: www.golem.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 01:30:29 2026 GMT
  host: learn.golem.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:39:03 2026 GMT
  host: release.api.golem.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Golem Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golem, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Golem
provider_slug: golem-cloud
slug: golem-cloud-domain-security
source_filename: golem-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.golem.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:02:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.golem.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:30:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: release.api.golem.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:39:03 2026 GMT\n  hsts: null\ndomains:\n- domain: golem.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/security/golem-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Durable Computing
- Serverless
- WebAssembly
- Workers
- Agents
---
