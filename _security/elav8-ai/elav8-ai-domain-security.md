---
api_specs:
- filename: elav8-ai-discovery-api-openapi.yml
  format: yaml
  label: ELAV8.ai Discovery API
  slug: elav8-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elav8-ai/openapi/elav8-ai-discovery-api-openapi.yml
- filename: elav8-ai-widget-runtime-api-openapi.yml
  format: yaml
  label: ELAV8.ai Widget runtime API
  slug: elav8-ai-widget-runtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elav8-ai/openapi/elav8-ai-widget-runtime-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elav8.ai
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: elav8.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ELAV8.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELAV8.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ELAV8.ai
provider_slug: elav8-ai
slug: elav8-ai-domain-security
source_filename: elav8-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elav8.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: elav8.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/elav8-ai/security/elav8-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Voice
- Productivity
- Conversations
---
