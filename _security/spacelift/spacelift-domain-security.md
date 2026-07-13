---
api_specs:
- filename: spacelift-openapi.yml
  format: yaml
  label: Spacelift GraphQL API
  slug: spacelift-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacelift/refs/heads/main/openapi/spacelift-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spacelift.io
  spf: true
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: spacelift.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacelift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spacelift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spacelift
provider_slug: spacelift
slug: spacelift-domain-security
source_filename: spacelift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacelift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spacelift.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacelift/refs/heads/main/security/spacelift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Infrastructure as Code
- FinOps
- DevOps
- Platform Engineering
- Terraform
- GitOps
---
