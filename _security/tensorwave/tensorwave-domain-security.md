---
api_specs:
- filename: tensorwave-generate-api-openapi.yml
  format: yaml
  label: TensorWave Generate API
  slug: tensorwave-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/openapi/tensorwave-generate-api-openapi.yml
- filename: tensorwave-health-api-openapi.yml
  format: yaml
  label: TensorWave Health API
  slug: tensorwave-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/openapi/tensorwave-health-api-openapi.yml
- filename: tensorwave-openai-api-openapi.yml
  format: yaml
  label: TensorWave Open AI API
  slug: tensorwave-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/openapi/tensorwave-openai-api-openapi.yml
- filename: tensorwave-slurm-api-openapi.yml
  format: yaml
  label: TensorWave Slurm API
  slug: tensorwave-slurm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/openapi/tensorwave-slurm-api-openapi.yml
- filename: tensorwave-training-api-openapi.yml
  format: yaml
  label: TensorWave Training API
  slug: tensorwave-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/openapi/tensorwave-training-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tensorwave.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: scalarlm.com
  spf: false
hosts:
- cert_expires: Oct 26 19:31:55 2026 GMT
  host: tensorwave.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 10:56:55 2026 GMT
  host: www.scalarlm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 08:43:02 2026 GMT
  host: gpt-oss.cray-lm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tensorwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TensorWave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TensorWave
provider_slug: tensorwave
slug: tensorwave-domain-security
source_filename: tensorwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tensorwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 19:31:55 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: www.scalarlm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:56:55 2026 GMT\n  hsts: false\n- host: gpt-oss.cray-lm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:43:02 2026 GMT\n  hsts: null\ndomains:\n- domain: tensorwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: scalarlm.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/security/tensorwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Cloud Computing
- GPU
- Infrastructure
- Inference
- Model Training
- High Performance Computing
- Data Centers
---
