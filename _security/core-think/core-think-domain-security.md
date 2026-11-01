---
api_specs:
- filename: core-think-openapi-generated.yml
  format: yaml
  label: Core Think API
  slug: core-think-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/core-think/openapi/_ae-authored/core-think-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corethink.ai
  spf: true
hosts:
- cert_expires: Dec 18 00:22:42 2026 GMT
  host: corethink.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Core Think Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Core Think, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Core Think
provider_slug: core-think
slug: core-think-domain-security
source_filename: core-think-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corethink.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 00:22:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: corethink.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/core-think/security/core-think-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Neurosymbolic
- Platform
- MachineLearning
---
