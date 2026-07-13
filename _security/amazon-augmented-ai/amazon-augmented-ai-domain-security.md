---
api_specs:
- filename: amazon-augmented-ai-openapi.yml
  format: yaml
  label: Amazon Augmented AI API
  slug: amazon-augmented-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-augmented-ai/refs/heads/main/openapi/amazon-augmented-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: a2i-runtime.sagemaker.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Augmented Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Augmented AI, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Augmented AI
provider_slug: amazon-augmented-ai
slug: amazon-augmented-ai-domain-security
source_filename: amazon-augmented-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: a2i-runtime.sagemaker.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-augmented-ai/refs/heads/main/security/amazon-augmented-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Augmented AI
- Human In The Loop
- Machine Learning
- AI Review
---
