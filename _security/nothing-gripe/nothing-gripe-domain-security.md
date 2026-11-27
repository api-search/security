---
api_specs:
- filename: nothing-gripe-agent-api-openapi.yml
  format: yaml
  label: Nothing.gripe Agent API
  slug: nothing-gripe-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothing-gripe/openapi/nothing-gripe-agent-api-openapi.yml
- filename: nothing-gripe-doer-api-openapi.yml
  format: yaml
  label: Nothing.gripe Doer API
  slug: nothing-gripe-doer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothing-gripe/openapi/nothing-gripe-doer-api-openapi.yml
- filename: nothing-gripe-tasks-api-openapi.yml
  format: yaml
  label: Nothing.gripe Tasks API
  slug: nothing-gripe-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothing-gripe/openapi/nothing-gripe-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nothing.gripe
  spf: true
hosts:
- cert_expires: Jan 26 14:25:22 2027 GMT
  host: nothing.gripe
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nothing.gripe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nothing.gripe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nothing.gripe
provider_slug: nothing-gripe
slug: nothing-gripe-domain-security
source_filename: nothing-gripe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nothing.gripe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 14:25:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nothing.gripe\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nothing-gripe/security/nothing-gripe-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Marketplace
- Task
- Cryptocurrency
- Funding
- Platform
- Company
---
