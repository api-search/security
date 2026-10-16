---
api_specs:
- filename: apizr-best-practices-openapi-generated.yml
  format: yaml
  label: APIZR best practices API
  slug: best-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/openapi/_ae-authored/apizr-best-practices-openapi-generated.yml
- filename: apizr-core-openapi-generated.yml
  format: yaml
  label: APIZR core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/openapi/_ae-authored/apizr-core-openapi-generated.yml
- filename: apizr-triggers-openapi-generated.yml
  format: yaml
  label: APIZR triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/openapi/_ae-authored/apizr-triggers-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apizr.fr
  spf: true
hosts:
- cert_expires: Jan  5 20:07:03 2027 GMT
  host: apizr.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apizr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIZR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APIZR
provider_slug: apizr
slug: apizr-domain-security
source_filename: apizr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apizr.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 20:07:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apizr.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/security/apizr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- iPaaS
- AI
- Integration
- Automation
- French
---
