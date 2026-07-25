---
api_specs:
- filename: astronomer-agenttoken-api-openapi.yml
  format: yaml
  label: Astronomer AgentToken API
  slug: astronomer-agenttoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-agenttoken-api-openapi.yml
- filename: astronomer-allowedipaddressrange-api-openapi.yml
  format: yaml
  label: Astronomer AllowedIpAddressRange API
  slug: astronomer-allowedipaddressrange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-allowedipaddressrange-api-openapi.yml
- filename: astronomer-apitoken-api-openapi.yml
  format: yaml
  label: Astronomer ApiToken API
  slug: astronomer-apitoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-apitoken-api-openapi.yml
- filename: astronomer-authorization-api-openapi.yml
  format: yaml
  label: Astronomer Authorization API
  slug: astronomer-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-authorization-api-openapi.yml
- filename: astronomer-cluster-api-openapi.yml
  format: yaml
  label: Astronomer Cluster API
  slug: astronomer-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-cluster-api-openapi.yml
- filename: astronomer-deploy-api-openapi.yml
  format: yaml
  label: Astronomer Deploy API
  slug: astronomer-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-deploy-api-openapi.yml
- filename: astronomer-deployment-api-openapi.yml
  format: yaml
  label: Astronomer Deployment API
  slug: astronomer-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-deployment-api-openapi.yml
- filename: astronomer-environment-api-openapi.yml
  format: yaml
  label: Astronomer Environment API
  slug: astronomer-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-environment-api-openapi.yml
- filename: astronomer-invite-api-openapi.yml
  format: yaml
  label: Astronomer Invite API
  slug: astronomer-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-invite-api-openapi.yml
- filename: astronomer-options-api-openapi.yml
  format: yaml
  label: Astronomer Options API
  slug: astronomer-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-options-api-openapi.yml
- filename: astronomer-organization-api-openapi.yml
  format: yaml
  label: Astronomer Organization API
  slug: astronomer-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-organization-api-openapi.yml
- filename: astronomer-role-api-openapi.yml
  format: yaml
  label: Astronomer Role API
  slug: astronomer-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-role-api-openapi.yml
- filename: astronomer-team-api-openapi.yml
  format: yaml
  label: Astronomer Team API
  slug: astronomer-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-team-api-openapi.yml
- filename: astronomer-user-api-openapi.yml
  format: yaml
  label: Astronomer User API
  slug: astronomer-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-user-api-openapi.yml
- filename: astronomer-workspace-api-openapi.yml
  format: yaml
  label: Astronomer Workspace API
  slug: astronomer-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astronomer.io
  spf: true
hosts:
- cert_expires: Sep 25 11:54:04 2026 GMT
  host: astronomer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 11:54:04 2026 GMT
  host: www.astronomer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.astronomer.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astronomer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astronomer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astronomer
provider_slug: astronomer
slug: astronomer-domain-security
source_filename: astronomer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astronomer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.astronomer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.astronomer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: astronomer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/security/astronomer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Orchestration
- Apache Airflow
- Data Pipelines
- Data Engineering
- Workflow Automation
- MLOps
- Managed Platform
---
