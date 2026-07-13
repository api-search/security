---
api_specs:
- filename: pipeline.swagger.json
  format: json
  label: Kubeflow Pipelines API
  slug: pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kubeflow/pipelines/master/backend/api/v2beta1/swagger/pipeline.swagger.json
- filename: rest_predict_v2.yaml
  format: yaml
  label: KServe Inference API
  slug: kserve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kserve/kserve/master/docs/predict-api/v2/rest_predict_v2.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kubeflow.org
  spf: false
hosts:
- cert_expires: Aug 25 10:09:17 2026 GMT
  host: www.kubeflow.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubeflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubeflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kubeflow
provider_slug: kubeflow
slug: kubeflow-domain-security
source_filename: kubeflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kubeflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:09:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubeflow.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeflow/refs/heads/main/security/kubeflow-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Deep Learning
- Kubernetes
- Machine Learning
- MLOps
- Model Serving
- Model Training
- Open Source
---
