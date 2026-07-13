---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Clarifai API
  slug: clarifai-api
  spec_type: OpenAPI
  url: https://api.clarifai.com/api-doc/?url=https://api.clarifai.com/v2/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clarifai.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.clarifai.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 27 15:25:18 2026 GMT
  host: docs.clarifai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.clarifai.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clarifai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarifai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clarifai
provider_slug: clarifai
slug: clarifai-domain-security
source_filename: clarifai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clarifai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\n- host: docs.clarifai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:25:18 2026 GMT\n  hsts: false\n- host: api.clarifai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: clarifai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarifai/refs/heads/main/security/clarifai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- AI
- Computer Vision
- NLP
- Image Recognition
- Object Detection
- Text Analysis
- Visual Search
- Machine Learning
- Custom Model Training
- gRPC
---
