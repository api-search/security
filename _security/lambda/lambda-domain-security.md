---
api_specs:
- filename: lambda-cloud-api-openapi.yml
  format: yaml
  label: Lambda Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/openapi/lambda-cloud-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lambda.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lambdalabs.com
  spf: true
hosts:
- cert_expires: Sep 25 02:35:14 2026 GMT
  host: lambda.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:00:59 2026 GMT
  host: docs.lambda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:12:03 2026 GMT
  host: cloud.lambdalabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lambda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lambda, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lambda
provider_slug: lambda
slug: lambda-domain-security
source_filename: lambda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:35:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:00:59 2026 GMT\n  hsts: false\n- host: cloud.lambdalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:12:03 2026 GMT\n  hsts: null\ndomains:\n- domain: lambda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lambdalabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/security/lambda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cloud Computing
- Compute
- Deep Learning
- GPU
- Machine Learning
---
