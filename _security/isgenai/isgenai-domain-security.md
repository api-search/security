---
api_specs:
- filename: isgenai-checks-api-openapi.yml
  format: yaml
  label: isGenAI Checks API
  slug: isgenai-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isgenai/openapi/isgenai-checks-api-openapi.yml
- filename: isgenai-content-credentials-api-openapi.yml
  format: yaml
  label: isGenAI Content Credentials API
  slug: isgenai-content-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isgenai/openapi/isgenai-content-credentials-api-openapi.yml
- filename: isgenai-health-api-openapi.yml
  format: yaml
  label: isGenAI Health API
  slug: isgenai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isgenai/openapi/isgenai-health-api-openapi.yml
- filename: isgenai-mcp-api-openapi.yml
  format: yaml
  label: isGenAI MCP API
  slug: isgenai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isgenai/openapi/isgenai-mcp-api-openapi.yml
- filename: isgenai-prompts-api-openapi.yml
  format: yaml
  label: isGenAI Prompts API
  slug: isgenai-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isgenai/openapi/isgenai-prompts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: isgenai.com
  spf: false
hosts:
- cert_expires: Dec  4 19:58:44 2026 GMT
  host: isgenai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Isgenai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for isGenAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: isGenAI
provider_slug: isgenai
slug: isgenai-domain-security
source_filename: isgenai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isgenai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 19:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: isgenai.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/isgenai/security/isgenai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Artificial Intelligence
- Detector
- Image
- Text
- Code
- Free
- Privacy
---
