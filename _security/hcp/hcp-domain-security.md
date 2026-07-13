---
api_specs:
- filename: hcp-openapi.yml
  format: yaml
  label: HCP Vault Secrets API
  slug: hcp-vault-secrets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
hosts:
- cert_expires: Aug 20 00:11:12 2026 GMT
  host: cloud.hashicorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.cloud.hashicorp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashiCorp Cloud Platform, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HashiCorp Cloud Platform
provider_slug: hcp
slug: hcp-domain-security
source_filename: hcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:11:12 2026 GMT\n  hsts: null\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cloud.hashicorp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/security/hcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Infrastructure
- DevOps
- Secrets Management
- Service Networking
- Fortune 1000
---
