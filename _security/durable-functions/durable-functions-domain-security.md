---
api_specs:
- filename: durable-functions-http-api-openapi.yml
  format: yaml
  label: Azure Durable Functions HTTP API
  slug: durable-functions-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/durable-functions/refs/heads/main/openapi/durable-functions-http-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Durable Functions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Durable Functions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Durable Functions
provider_slug: durable-functions
slug: durable-functions-domain-security
source_filename: durable-functions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/durable-functions/refs/heads/main/security/durable-functions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Composition
- Durable Execution
- Serverless Orchestration
- Workflow
---
