---
api_specs:
- filename: kubecost-allocation-openapi.yml
  format: yaml
  label: Kubecost Allocation API
  slug: allocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-allocation-openapi.yml
- filename: kubecost-assets-openapi.yml
  format: yaml
  label: Kubecost Assets API
  slug: assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-assets-openapi.yml
- filename: kubecost-cloud-cost-openapi.yml
  format: yaml
  label: Kubecost Cloud Cost API
  slug: cloud-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-cloud-cost-openapi.yml
- filename: kubecost-budget-openapi.yml
  format: yaml
  label: Kubecost Budget API
  slug: budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-budget-openapi.yml
- filename: kubecost-forecast-openapi.yml
  format: yaml
  label: Kubecost Forecast API
  slug: forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-forecast-openapi.yml
- filename: kubecost-savings-openapi.yml
  format: yaml
  label: Kubecost Savings API
  slug: savings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-savings-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kubecost.com
  spf: true
hosts:
- cert_expires: Aug 23 11:21:50 2026 GMT
  host: docs.kubecost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubecost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubecost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kubecost
provider_slug: kubecost
slug: kubecost-domain-security
source_filename: kubecost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.kubecost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:21:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubecost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/security/kubecost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
---
