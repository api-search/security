---
api_specs:
- filename: terraform-modules-api-openapi.yml
  format: yaml
  label: Terraform Modules API
  slug: terraform-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-modules-api-openapi.yml
- filename: terraform-organizations-api-openapi.yml
  format: yaml
  label: Terraform Organizations API
  slug: terraform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-organizations-api-openapi.yml
- filename: terraform-policies-api-openapi.yml
  format: yaml
  label: Terraform Policies API
  slug: terraform-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-policies-api-openapi.yml
- filename: terraform-projects-api-openapi.yml
  format: yaml
  label: Terraform Projects API
  slug: terraform-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-projects-api-openapi.yml
- filename: terraform-runs-api-openapi.yml
  format: yaml
  label: Terraform Runs API
  slug: terraform-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-runs-api-openapi.yml
- filename: terraform-state-versions-api-openapi.yml
  format: yaml
  label: Terraform State Versions API
  slug: terraform-state-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-state-versions-api-openapi.yml
- filename: terraform-teams-api-openapi.yml
  format: yaml
  label: Terraform Teams API
  slug: terraform-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-teams-api-openapi.yml
- filename: terraform-variables-api-openapi.yml
  format: yaml
  label: Terraform Variables API
  slug: terraform-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-variables-api-openapi.yml
- filename: terraform-workspaces-api-openapi.yml
  format: yaml
  label: Terraform Workspaces API
  slug: terraform-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terraform.io
  spf: true
hosts:
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: registry.terraform.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: app.terraform.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terraform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terraform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terraform
provider_slug: terraform
slug: terraform-domain-security
source_filename: terraform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: registry.terraform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.terraform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: terraform.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/security/terraform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Infrastructure As Code
- Cloud Infrastructure
- DevOps
- Open-Source
- HashiCorp
---
