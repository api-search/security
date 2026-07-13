---
api_specs:
- filename: pipeline.swagger.json
  format: json
  label: Kubeflow Pipelines REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kubeflow/pipelines/master/backend/api/v2beta1/swagger/pipeline.swagger.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kubeflow.org
  spf: false
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug 25 10:09:17 2026 GMT
  host: www.kubeflow.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: kubeflow-pipelines.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubeflow Pipelines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubeflow Pipelines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Kubeflow Pipelines
provider_slug: kubeflow-pipelines
slug: kubeflow-pipelines-domain-security
source_filename: kubeflow-pipelines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kubeflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:09:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kubeflow-pipelines.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubeflow.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeflow-pipelines/refs/heads/main/security/kubeflow-pipelines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Data Science
- Kubernetes
- Machine Learning
- MLOps
- Orchestration
- Pipelines
- Workflows
---
