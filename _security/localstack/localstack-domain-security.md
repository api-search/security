---
api_specs:
- filename: localstack-openapi-original.yml
  format: yaml
  label: LocalStack REST API for Community
  slug: localstack-rest-api-for-community
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localstack/refs/heads/main/openapi/localstack-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: localstack.cloud
  spf: true
hosts:
- cert_expires: Oct  1 19:03:27 2026 GMT
  host: www.localstack.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocalStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LocalStack
provider_slug: localstack
slug: localstack-domain-security
source_filename: localstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.localstack.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:03:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: localstack.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localstack/refs/heads/main/security/localstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Cloud
- Emulator
- Testing
- DevOps
- Serverless
- Infrastructure
---
