---
api_specs:
- filename: adaption-labs-datasets-api-openapi.yml
  format: yaml
  label: Adaption Labs Datasets API
  slug: adaption-labs-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/openapi/adaption-labs-datasets-api-openapi.yml
- filename: adaption-labs-upload-api-openapi.yml
  format: yaml
  label: Adaption Labs Upload API
  slug: adaption-labs-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/openapi/adaption-labs-upload-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adaptionlabs.ai
  spf: true
hosts:
- cert_expires: Oct 13 17:26:40 2026 GMT
  host: www.adaptionlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adaption Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaption Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adaption Labs
provider_slug: adaption-labs
slug: adaption-labs-domain-security
source_filename: adaption-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adaptionlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:26:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adaptionlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/security/adaption-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Training Data
- Datasets
- LLM
- Adaptive Data
- SDK
---
