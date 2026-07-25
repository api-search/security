---
api_specs:
- filename: turbonomic-actions-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Actions API
  slug: turbonomic-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-actions-api-openapi.yml
- filename: turbonomic-authentication-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Authentication API
  slug: turbonomic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-authentication-api-openapi.yml
- filename: turbonomic-entities-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Entities API
  slug: turbonomic-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-entities-api-openapi.yml
- filename: turbonomic-groups-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Groups API
  slug: turbonomic-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-groups-api-openapi.yml
- filename: turbonomic-markets-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Markets API
  slug: turbonomic-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-markets-api-openapi.yml
- filename: turbonomic-policies-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Policies API
  slug: turbonomic-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-policies-api-openapi.yml
- filename: turbonomic-statistics-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Statistics API
  slug: turbonomic-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-statistics-api-openapi.yml
- filename: turbonomic-targets-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Targets API
  slug: turbonomic-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-targets-api-openapi.yml
- filename: turbonomic-templates-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Templates API
  slug: turbonomic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-templates-api-openapi.yml
- filename: turbonomic-topology-api-openapi.yml
  format: yaml
  label: IBM Turbonomic Topology API
  slug: turbonomic-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/openapi/turbonomic-topology-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.ibm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turbonomic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBM Turbonomic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IBM Turbonomic
provider_slug: turbonomic
slug: turbonomic-domain-security
source_filename: turbonomic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbonomic/refs/heads/main/security/turbonomic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Resource Management
- Cloud Cost Optimization
- Cloud Management
- Hybrid Cloud
- IBM
- Kubernetes
- Multi-Cloud
- Workload Optimization
---
