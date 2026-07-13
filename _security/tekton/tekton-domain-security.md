---
api_specs:
- filename: tekton-pipeline-openapi.json
  format: json
  label: Tekton Task CRD
  slug: tekton-task-crd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekton/refs/heads/main/openapi/tekton-pipeline-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tekton.dev
  spf: false
hosts:
- cert_expires: Aug 15 20:39:50 2026 GMT
  host: tekton.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tekton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tekton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tekton
provider_slug: tekton
slug: tekton-domain-security
source_filename: tekton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tekton.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 20:39:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tekton.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekton/refs/heads/main/security/tekton-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- DevOps
- CI/CD
- Kubernetes
- CNCF
- Pipelines
- Open Source
- CRD
- Operator
---
