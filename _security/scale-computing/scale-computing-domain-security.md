---
api_specs:
- filename: scale-computing-api-keys-api-openapi.yml
  format: yaml
  label: Scale Computing API Keys API
  slug: scale-computing-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-api-keys-api-openapi.yml
- filename: scale-computing-clusters-api-openapi.yml
  format: yaml
  label: Scale Computing Clusters API
  slug: scale-computing-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-clusters-api-openapi.yml
- filename: scale-computing-conditions-api-openapi.yml
  format: yaml
  label: Scale Computing Conditions API
  slug: scale-computing-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-conditions-api-openapi.yml
- filename: scale-computing-health-api-openapi.yml
  format: yaml
  label: Scale Computing Health API
  slug: scale-computing-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-health-api-openapi.yml
- filename: scale-computing-metrics-api-openapi.yml
  format: yaml
  label: Scale Computing Metrics API
  slug: scale-computing-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-metrics-api-openapi.yml
- filename: scale-computing-nodes-api-openapi.yml
  format: yaml
  label: Scale Computing Nodes API
  slug: scale-computing-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-nodes-api-openapi.yml
- filename: scale-computing-organization-activities-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Activities API
  slug: scale-computing-organization-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-activities-api-openapi.yml
- filename: scale-computing-organization-api-openapi.yml
  format: yaml
  label: Scale Computing Organization API
  slug: scale-computing-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-api-openapi.yml
- filename: scale-computing-organization-salesforce-account-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Salesforce Account API
  slug: scale-computing-organization-salesforce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-salesforce-account-api-openapi.yml
- filename: scale-computing-organizationroles-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Roles API
  slug: scale-computing-organizationroles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationroles-api-openapi.yml
- filename: scale-computing-organizations-api-openapi.yml
  format: yaml
  label: Scale Computing Organizations API
  slug: scale-computing-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizations-api-openapi.yml
- filename: scale-computing-organizationuser-api-openapi.yml
  format: yaml
  label: Scale Computing Organization User API
  slug: scale-computing-organizationuser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationuser-api-openapi.yml
- filename: scale-computing-organizationusers-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Users API
  slug: scale-computing-organizationusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationusers-api-openapi.yml
- filename: scale-computing-salesforce-api-openapi.yml
  format: yaml
  label: Scale Computing Salesforce API
  slug: scale-computing-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-salesforce-api-openapi.yml
- filename: scale-computing-staged-clusters-api-openapi.yml
  format: yaml
  label: Scale Computing Staged Clusters API
  slug: scale-computing-staged-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-staged-clusters-api-openapi.yml
- filename: scale-computing-users-api-openapi.yml
  format: yaml
  label: Scale Computing Users API
  slug: scale-computing-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-users-api-openapi.yml
- filename: scale-computing-vms-api-openapi.yml
  format: yaml
  label: Scale Computing Vms API
  slug: scale-computing-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-vms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scalecomputing.com
  spf: true
hosts:
- cert_expires: Oct 18 08:13:39 2026 GMT
  host: www.scalecomputing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 21:07:17 2026 GMT
  host: api.scalecomputing.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scale Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scale Computing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scale Computing
provider_slug: scale-computing
slug: scale-computing-domain-security
source_filename: scale-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scalecomputing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 08:13:39 2026 GMT\n  hsts: false\n- host: api.scalecomputing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 21:07:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scalecomputing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/security/scale-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Edge Computing
- Hyperconverged Infrastructure
- Virtualization
- Infrastructure Management
- Fleet Management
- Virtual Machines
- Observability
- Infrastructure as Code
- Kubernetes
- Company
---
