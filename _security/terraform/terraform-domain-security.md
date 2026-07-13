---
api_specs:
- filename: hcp-terraform-openapi.yml
  format: yaml
  label: HCP Terraform API
  slug: hcp-terraform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/hcp-terraform-openapi.yml
- filename: terraform-registry-openapi.yml
  format: yaml
  label: Terraform Registry API
  slug: terraform-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-registry-openapi.yml
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
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: registry.terraform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.terraform.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: terraform.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/security/terraform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Infrastructure As Code
- Cloud Infrastructure
- DevOps
- Open Source
- HashiCorp
---
