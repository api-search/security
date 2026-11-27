---
api_specs:
- filename: korey-ai-identity-api-openapi.yml
  format: yaml
  label: Korey Identity API
  slug: korey-ai-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korey-ai/openapi/korey-ai-identity-api-openapi.yml
- filename: korey-ai-threads-api-openapi.yml
  format: yaml
  label: Korey Threads API
  slug: korey-ai-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korey-ai/openapi/korey-ai-threads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: korey.ai
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: korey.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Korey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Korey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Korey
provider_slug: korey-ai
slug: korey-ai-domain-security
source_filename: korey-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: korey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: korey.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/korey-ai/security/korey-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- Product Teams
- Approval Workflow
- Collaboration
---
