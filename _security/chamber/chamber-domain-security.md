---
api_specs:
- filename: chamber-capacity-api-openapi.yml
  format: yaml
  label: Chamber Capacity API
  slug: chamber-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-capacity-api-openapi.yml
- filename: chamber-health-api-openapi.yml
  format: yaml
  label: Chamber Health API
  slug: chamber-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-health-api-openapi.yml
- filename: chamber-metrics-api-openapi.yml
  format: yaml
  label: Chamber Metrics API
  slug: chamber-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-metrics-api-openapi.yml
- filename: chamber-workloads-api-openapi.yml
  format: yaml
  label: Chamber Workloads API
  slug: chamber-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/openapi/chamber-workloads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: usechamber.io
  spf: false
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api.usechamber.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chamber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chamber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Chamber
provider_slug: chamber
slug: chamber-domain-security
source_filename: chamber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.usechamber.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usechamber.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chamber/refs/heads/main/security/chamber-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- GPU
- AIOps
- Machine Learning
- MLOps
- Infrastructure
- Cloud
- Kubernetes
- Observability
- Monitoring
- Company
---
