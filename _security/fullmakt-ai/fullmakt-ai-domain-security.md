---
api_specs:
- filename: fullmakt-ai-openapi-generated.yml
  format: yaml
  label: Fullmakt API
  slug: fullmakt-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fullmakt-ai/openapi/_ae-authored/fullmakt-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fullmakt.ai
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: fullmakt.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fullmakt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fullmakt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fullmakt
provider_slug: fullmakt-ai
slug: fullmakt-ai-domain-security
source_filename: fullmakt-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fullmakt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: fullmakt.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fullmakt-ai/security/fullmakt-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Security
- Credential Broker
- API Management
- Software-as-a-Service
---
