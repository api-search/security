---
api_specs:
- filename: dynamo-ai-dynamo-ai-api-api-openapi.yml
  format: yaml
  label: Dynamo AI API
  slug: dynamo-ai-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamo-ai/openapi/dynamo-ai-dynamo-ai-api-api-openapi.yml
- filename: dynamo-ai-openapi-generated.yml
  format: yaml
  label: Dynamo AI API
  slug: dynamo-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamo-ai/openapi/_ae-authored/dynamo-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Jan 13 02:07:18 2027 GMT
  host: forgeglobal.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynamo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamo AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dynamo AI
provider_slug: dynamo-ai
slug: dynamo-ai-domain-security
source_filename: dynamo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 02:07:18 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dynamo-ai/security/dynamo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Security
- Enterprise
- Compliance
---
