---
api_specs:
- filename: kubernetes-autoscaling-api-openapi.yml
  format: yaml
  label: Kubernetes Autoscaling API
  slug: kubernetes-autoscaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-autoscaling-api-openapi.yml
- filename: kubernetes-cluster-api-openapi.yml
  format: yaml
  label: Kubernetes Cluster API
  slug: kubernetes-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-cluster-api-openapi.yml
- filename: kubernetes-config-api-openapi.yml
  format: yaml
  label: Kubernetes Config API
  slug: kubernetes-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-config-api-openapi.yml
- filename: kubernetes-events-api-openapi.yml
  format: yaml
  label: Kubernetes Events API
  slug: kubernetes-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-events-api-openapi.yml
- filename: kubernetes-namespaces-api-openapi.yml
  format: yaml
  label: Kubernetes Namespaces API
  slug: kubernetes-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-namespaces-api-openapi.yml
- filename: kubernetes-rbac-api-openapi.yml
  format: yaml
  label: Kubernetes RBAC API
  slug: kubernetes-rbac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-rbac-api-openapi.yml
- filename: kubernetes-workloads-api-openapi.yml
  format: yaml
  label: Kubernetes Workloads API
  slug: kubernetes-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/openapi/kubernetes-workloads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kubernetes.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Sep 11 09:13:55 2026 GMT
  host: kubernetes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Kubernetes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubernetes, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kubernetes
provider_slug: kubernetes
slug: kubernetes-domain-security
source_filename: kubernetes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubernetes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: kubernetes.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubernetes/refs/heads/main/security/kubernetes-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automation
- Cloud Native
- CNCF
- Containers
- Deployment
- Open Source
- Orchestration
- Scaling
---
