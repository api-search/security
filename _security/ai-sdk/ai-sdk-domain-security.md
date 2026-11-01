---
api_specs:
- filename: ai-sdk-openapi-generated.yml
  format: yaml
  label: Google API
  slug: ai-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-sdk/openapi/_ae-authored/ai-sdk-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Dec 21 18:38:32 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ai Sdk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google
provider_slug: ai-sdk
slug: ai-sdk-domain-security
source_filename: ai-sdk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 18:38:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ai-sdk/security/ai-sdk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Cloud
- Machine Learning
- SDK
---
