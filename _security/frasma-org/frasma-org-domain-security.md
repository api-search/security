---
api_specs:
- filename: frasma-org-chat-api-openapi.yml
  format: yaml
  label: Frasma Chat API
  slug: frasma-org-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frasma-org/openapi/frasma-org-chat-api-openapi.yml
- filename: frasma-org-conversations-api-openapi.yml
  format: yaml
  label: Frasma Conversations API
  slug: frasma-org-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frasma-org/openapi/frasma-org-conversations-api-openapi.yml
- filename: frasma-org-mcp-api-openapi.yml
  format: yaml
  label: Frasma MCP API
  slug: frasma-org-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frasma-org/openapi/frasma-org-mcp-api-openapi.yml
- filename: frasma-org-request-process-assessment-api-openapi.yml
  format: yaml
  label: Frasma Request Process Assessment API
  slug: frasma-org-request-process-assessment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frasma-org/openapi/frasma-org-request-process-assessment-api-openapi.yml
- filename: frasma-org-status-api-openapi.yml
  format: yaml
  label: Frasma Status API
  slug: frasma-org-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frasma-org/openapi/frasma-org-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: frasma.org
  spf: true
hosts:
- cert_expires: Dec 29 23:31:13 2026 GMT
  host: frasma.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:31:13 2026 GMT
  host: www.frasma.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Frasma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frasma, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Frasma
provider_slug: frasma-org
slug: frasma-org-domain-security
source_filename: frasma-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frasma.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:31:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.frasma.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:31:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: frasma.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/frasma-org/security/frasma-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Document Management
- ERP Integration
- Italian SME
- Business Process
---
