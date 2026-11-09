---
api_specs:
- filename: deepskyai-com-compliance-api-openapi.yml
  format: yaml
  label: Deepsky Compliance API
  slug: deepskyai-com-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-compliance-api-openapi.yml
- filename: deepskyai-com-deepsky-aviation-agent-api-api-openapi.yml
  format: yaml
  label: Deepsky Deepsky Aviation Agent API
  slug: deepskyai-com-deepsky-aviation-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-deepsky-aviation-agent-api-api-openapi.yml
- filename: deepskyai-com-mcp-api-openapi.yml
  format: yaml
  label: Deepsky MCP API
  slug: deepskyai-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-mcp-api-openapi.yml
- filename: deepskyai-com-search-api-openapi.yml
  format: yaml
  label: Deepsky Search API
  slug: deepskyai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-search-api-openapi.yml
- filename: deepskyai-com-skills-api-openapi.yml
  format: yaml
  label: Deepsky Skills API
  slug: deepskyai-com-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-skills-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepskyai.com
  spf: false
hosts:
- cert_expires: Dec 23 10:18:08 2026 GMT
  host: deepskyai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deepskyai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepsky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Deepsky
provider_slug: deepskyai-com
slug: deepskyai-com-domain-security
source_filename: deepskyai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepskyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 10:18:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deepskyai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deepskyai-com/security/deepskyai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Artificial Intelligence
- Automation
- Documentation
- Compliance
- Company
---
