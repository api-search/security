---
api_specs:
- filename: harness-cloud-cost-anomalies-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Anomalies API
  slug: harness-cloud-cost-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-anomalies-api-openapi.yml
- filename: harness-cloud-cost-budgets-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Budgets API
  slug: harness-cloud-cost-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-budgets-api-openapi.yml
- filename: harness-cloud-cost-connectors-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Connectors API
  slug: harness-cloud-cost-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-connectors-api-openapi.yml
- filename: harness-cloud-cost-cost-categories-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Cost Categories API
  slug: harness-cloud-cost-cost-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-cost-categories-api-openapi.yml
- filename: harness-cloud-cost-perspectives-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Perspectives API
  slug: harness-cloud-cost-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-perspectives-api-openapi.yml
- filename: harness-cloud-cost-recommendations-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Recommendations API
  slug: harness-cloud-cost-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-recommendations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harness.io
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.harness.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: app.harness.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harness Cloud Cost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harness Cloud Cost Management, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harness Cloud Cost Management
provider_slug: harness-cloud-cost
slug: harness-cloud-cost-domain-security
source_filename: harness-cloud-cost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harness.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.harness.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: harness.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/security/harness-cloud-cost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anomaly Detection
- Budgets
- Cloud Cost Management
- FinOps
- Kubernetes
- Recommendations
---
