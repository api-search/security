---
api_specs:
- filename: ternary-anomaly-detection-api-openapi.yml
  format: yaml
  label: Ternary Anomaly Detection API
  slug: ternary-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-anomaly-detection-api-openapi.yml
- filename: ternary-commitments-api-openapi.yml
  format: yaml
  label: Ternary Commitments API
  slug: ternary-commitments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-commitments-api-openapi.yml
- filename: ternary-cost-allocation-api-openapi.yml
  format: yaml
  label: Ternary Cost Allocation API
  slug: ternary-cost-allocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-cost-allocation-api-openapi.yml
- filename: ternary-forecasting-api-openapi.yml
  format: yaml
  label: Ternary Forecasting API
  slug: ternary-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-forecasting-api-openapi.yml
- filename: ternary-kubernetes-api-openapi.yml
  format: yaml
  label: Ternary Kubernetes API
  slug: ternary-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-kubernetes-api-openapi.yml
- filename: ternary-reporting-api-openapi.yml
  format: yaml
  label: Ternary Reporting API
  slug: ternary-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/openapi/ternary-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ternary.app
  spf: true
hosts:
- cert_expires: Aug 20 03:48:44 2026 GMT
  host: ternary.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 03:27:50 2026 GMT
  host: api.ternary.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ternary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ternary, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ternary
provider_slug: ternary
slug: ternary-domain-security
source_filename: ternary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ternary.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 03:48:44 2026 GMT\n  hsts: false\n- host: api.ternary.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:27:50 2026 GMT\n  hsts: null\ndomains:\n- domain: ternary.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ternary/refs/heads/main/security/ternary-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Cost Management
- Cost Optimization
- FinOps
- Google Cloud
- Kubernetes
- Multi-Cloud
---
