---
api_specs:
- filename: helm-chart-repository-openapi.yml
  format: yaml
  label: Helm Chart Repository API
  slug: chart-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helm/refs/heads/main/openapi/helm-chart-repository-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: helm.sh
  spf: false
hosts:
- cert_expires: Sep 24 20:44:10 2026 GMT
  host: helm.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Helm
provider_slug: helm
slug: helm-domain-security
source_filename: helm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helm.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helm.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helm/refs/heads/main/security/helm-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Charts
- Cloud Native
- Container Orchestration
- DevOps
- Kubernetes
- Package Manager
---
