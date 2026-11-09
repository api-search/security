---
api_specs:
- filename: ilang-ai-agent-api-openapi.yml
  format: yaml
  label: iLang Agent API
  slug: ilang-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ilang-ai/openapi/ilang-ai-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ilang.ai
  spf: true
hosts:
- cert_expires: Jan 23 19:16:09 2027 GMT
  host: ilang.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ilang Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iLang, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: iLang
provider_slug: ilang-ai
slug: ilang-ai-domain-security
source_filename: ilang-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ilang.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 19:16:09 2027 GMT\n  hsts: false\ndomains:\n- domain: ilang.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ilang-ai/security/ilang-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Protocol
- Open Source
- Interoperability
---
