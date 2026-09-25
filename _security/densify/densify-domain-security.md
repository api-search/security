---
api_specs:
- filename: densify-analysis-webhook-api-openapi.yml
  format: yaml
  label: Densify Analysis Webhook API
  slug: densify-analysis-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-analysis-webhook-api-openapi.yml
- filename: densify-authentication-api-openapi.yml
  format: yaml
  label: Densify Authentication API
  slug: densify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-authentication-api-openapi.yml
- filename: densify-aws-analysis-api-openapi.yml
  format: yaml
  label: Densify AWS Analysis API
  slug: densify-aws-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-aws-analysis-api-openapi.yml
- filename: densify-aws-analyze-api-openapi.yml
  format: yaml
  label: Densify AWS Analyze API
  slug: densify-aws-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-aws-analyze-api-openapi.yml
- filename: densify-azure-analysis-api-openapi.yml
  format: yaml
  label: Densify Azure Analysis API
  slug: densify-azure-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-azure-analysis-api-openapi.yml
- filename: densify-cloud-analysis-api-openapi.yml
  format: yaml
  label: Densify Cloud Analysis API
  slug: densify-cloud-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-cloud-analysis-api-openapi.yml
- filename: densify-gcp-analysis-api-openapi.yml
  format: yaml
  label: Densify GCP Analysis API
  slug: densify-gcp-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-gcp-analysis-api-openapi.yml
- filename: densify-kubernetes-api-openapi.yml
  format: yaml
  label: Densify Kubernetes API
  slug: densify-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-api-openapi.yml
- filename: densify-kubernetes-cluster-results-api-openapi.yml
  format: yaml
  label: Densify Kubernetes Cluster Results API
  slug: densify-kubernetes-cluster-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-cluster-results-api-openapi.yml
- filename: densify-kubernetes-clusters-api-openapi.yml
  format: yaml
  label: Densify Kubernetes Clusters API
  slug: densify-kubernetes-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-clusters-api-openapi.yml
- filename: densify-recommendations-api-openapi.yml
  format: yaml
  label: Densify Recommendations API
  slug: densify-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-recommendations-api-openapi.yml
- filename: densify-subscriptions-api-openapi.yml
  format: yaml
  label: Densify Subscriptions API
  slug: densify-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-api-openapi.yml
- filename: densify-subscriptions-properties-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Properties API
  slug: densify-subscriptions-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-properties-api-openapi.yml
- filename: densify-subscriptions-suppressions-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Suppressions API
  slug: densify-subscriptions-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-suppressions-api-openapi.yml
- filename: densify-subscriptions-tags-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Tags API
  slug: densify-subscriptions-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-tags-api-openapi.yml
- filename: densify-system-api-openapi.yml
  format: yaml
  label: Densify System API
  slug: densify-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-system-api-openapi.yml
- filename: densify-systems-api-openapi.yml
  format: yaml
  label: Densify Systems API
  slug: densify-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-systems-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: densify.com
  spf: true
hosts:
- cert_expires: Oct 17 02:54:26 2026 GMT
  host: www.densify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:54:26 2026 GMT
  host: portal.densify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:54:26 2026 GMT
  host: api.densify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Densify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Densify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Densify
provider_slug: densify
slug: densify-domain-security
source_filename: densify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.densify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:54:26 2026 GMT\n  hsts: false\n- host: portal.densify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:54:26 2026 GMT\n  hsts: false\n- host: api.densify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:54:26 2026 GMT\n  hsts: false\ndomains:\n- domain: densify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/security/densify-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud Cost
- Container Optimization
- FinOps
- Kubernetes
- Machine Learning
- Recommendations
- Rightsizing
- A2A
---
