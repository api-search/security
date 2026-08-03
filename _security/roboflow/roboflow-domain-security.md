---
api_specs:
- filename: roboflow-inference-openapi.json
  format: json
  label: Roboflow Inference Server API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roboflow/refs/heads/main/openapi/roboflow-inference-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: roboflow.com
  spf: true
hosts:
- cert_expires: Oct  3 06:24:26 2026 GMT
  host: roboflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 03:33:23 2026 GMT
  host: docs.roboflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 20:09:25 2026 GMT
  host: serverless.roboflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roboflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roboflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Roboflow
provider_slug: roboflow
slug: roboflow-domain-security
source_filename: roboflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roboflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:24:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.roboflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 03:33:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: serverless.roboflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:09:25 2026 GMT\n  hsts: false\ndomains:\n- domain: roboflow.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roboflow/refs/heads/main/security/roboflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Computer Vision
- Machine Learning
- Artificial Intelligence
- Object Detection
- Image Annotation
- Model Training
- Inference
- MLOps
- Edge AI
- Datasets
---
