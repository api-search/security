---
api_specs:
- filename: bentoml-bentocloud-deployment-api-openapi.yml
  format: yaml
  label: BentoCloud Deployment API
  slug: bentocloud-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bentoml/refs/heads/main/openapi/bentoml-bentocloud-deployment-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bentoml.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.bentoml.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 09:47:21 2026 GMT
  host: docs.bentoml.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: cloud.bentoml.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bentoml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BentoML, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BentoML
provider_slug: bentoml
slug: bentoml-domain-security
source_filename: bentoml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bentoml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bentoml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:47:21 2026 GMT\n  hsts: false\n- host: cloud.bentoml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: bentoml.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bentoml/refs/heads/main/security/bentoml-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- machine learning
- model serving
- inference
- AI
- REST API
- MLOps
- deployment
- GPU
- LLM
- BentoCloud
---
