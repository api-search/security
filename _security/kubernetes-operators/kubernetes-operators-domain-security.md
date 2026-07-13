---
api_specs:
- filename: kubernetes-operators-watch-asyncapi.yml
  format: yaml
  label: Kubernetes Operators
  slug: kubernetes-operators
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-operators/refs/heads/main/asyncapi/kubernetes-operators-watch-asyncapi.yml
- filename: kubernetes-crd-openapi.yml
  format: yaml
  label: Kubernetes Custom Resource Definitions
  slug: custom-resource-definitions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-operators/refs/heads/main/openapi/kubernetes-crd-openapi.yml
- filename: kubernetes-olm-openapi.yml
  format: yaml
  label: Operator Lifecycle Manager
  slug: operator-lifecycle-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes-operators/refs/heads/main/openapi/kubernetes-olm-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: kubernetes.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: operatorframework.io
  spf: false
hosts:
- cert_expires: Sep 11 09:13:55 2026 GMT
  host: kubernetes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:59:54 2026 GMT
  host: sdk.operatorframework.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:59:54 2026 GMT
  host: olm.operatorframework.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubernetes Operators Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubernetes Operators, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kubernetes Operators
provider_slug: kubernetes-operators
slug: kubernetes-operators-domain-security
source_filename: kubernetes-operators-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubernetes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sdk.operatorframework.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:59:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: olm.operatorframework.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:59:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubernetes.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n- domain: operatorframework.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubernetes-operators/refs/heads/main/security/kubernetes-operators-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automation
- Cloud Native
- DevOps
- Infrastructure
- Kubernetes
---
