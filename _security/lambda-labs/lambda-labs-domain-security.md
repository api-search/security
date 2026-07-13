---
api_specs:
- filename: lambda-labs-openapi.json
  format: json
  label: Lambda Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-openapi.json
- filename: lambda-labs-asyncapi.yml
  format: yaml
  label: Lambda Inference API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/asyncapi/lambda-labs-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lambda.ai
  spf: true
hosts:
- cert_expires: Sep 25 02:35:14 2026 GMT
  host: lambda.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 06:14:15 2026 GMT
  host: cloud.lambda.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:00:59 2026 GMT
  host: docs.lambda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lambda Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lambda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lambda
provider_slug: lambda-labs
slug: lambda-labs-domain-security
source_filename: lambda-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:35:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:14:15 2026 GMT\n  hsts: null\n- host: docs.lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:00:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lambda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/security/lambda-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cloud
- Clusters
- Compute
- GPU
- Inference
- Machine Learning
---
