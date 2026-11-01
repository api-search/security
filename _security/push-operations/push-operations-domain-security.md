---
api_specs:
- filename: push-operations-openapi-generated.yml
  format: yaml
  label: Push Operations API
  slug: push-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/push-operations/openapi/_ae-authored/push-operations-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pushoperations.com
  spf: true
hosts:
- cert_expires: Jan  6 10:38:29 2027 GMT
  host: pushoperations.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Push Operations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Push Operations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Push Operations
provider_slug: push-operations
slug: push-operations-domain-security
source_filename: push-operations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pushoperations.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 10:38:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pushoperations.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/push-operations/security/push-operations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payroll
- HR
- Workforce Management
- SaaS
- Hospitality
- Company
---
