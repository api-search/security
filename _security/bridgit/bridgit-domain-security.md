---
api_specs:
- filename: bridgit-bench-openapi.yml
  format: yaml
  label: Bridgit Bench API
  slug: bridgit-bench
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridgit/refs/heads/main/openapi/bridgit-bench-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gobridgit.com
  spf: true
hosts:
- cert_expires: Sep  6 20:28:05 2026 GMT
  host: gobridgit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: bench.gobridgit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bridgit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridgit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bridgit
provider_slug: bridgit
slug: bridgit-domain-security
source_filename: bridgit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gobridgit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 20:28:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bench.gobridgit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gobridgit.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgit/refs/heads/main/security/bridgit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Construction Technology
- Workforce Planning
- Workforce Management
- Resource Planning
- Project Staffing
- General Contractors
- Subcontractors
- Forecasting
- Utilization
- Certifications
- AEC
- SaaS
---
