---
api_specs:
- filename: semaphore-semaphore-api-openapi.yml
  format: yaml
  label: Semaphore API
  slug: semaphore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-semaphore-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: semaphore.io
  spf: true
hosts:
- cert_expires: Aug 31 11:03:05 2026 GMT
  host: semaphore.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Semaphore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semaphore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Semaphore
provider_slug: semaphore
slug: semaphore-domain-security
source_filename: semaphore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: semaphore.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:03:05 2026 GMT\n  hsts: false\ndomains:\n- domain: semaphore.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/security/semaphore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- Pipelines
- Workflows
- DevOps
- Build Automation
- Software Delivery
- Deployment
- Artifacts
---
