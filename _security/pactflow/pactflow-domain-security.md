---
api_specs:
- filename: pactflow-openapi-generated.yml
  format: yaml
  label: PactFlow API
  slug: pactflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pactflow/refs/heads/main/openapi/_ae-authored/pactflow-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pactflow.io
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: pactflow.io
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pactflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PactFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PactFlow
provider_slug: pactflow
slug: pactflow-domain-security
source_filename: pactflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pactflow.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10368000\ndomains:\n- domain: pactflow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pactflow/refs/heads/main/security/pactflow-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- API Testing
- Contract Testing
- Microservices
- CI/CD
---
