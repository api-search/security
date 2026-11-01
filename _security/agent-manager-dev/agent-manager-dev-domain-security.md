---
api_specs:
- filename: agent-manager-dev-docs-api-openapi.yml
  format: yaml
  label: agent-manager-dev Docs API
  slug: agent-manager-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-docs-api-openapi.yml
- filename: agent-manager-dev-meta-api-openapi.yml
  format: yaml
  label: agent-manager-dev Meta API
  slug: agent-manager-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-meta-api-openapi.yml
- filename: agent-manager-dev-product-api-openapi.yml
  format: yaml
  label: agent-manager-dev Product API
  slug: agent-manager-dev-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-product-api-openapi.yml
- filename: agent-manager-dev-releases-api-openapi.yml
  format: yaml
  label: agent-manager-dev Releases API
  slug: agent-manager-dev-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-releases-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agent-manager.dev
  spf: true
hosts:
- cert_expires: Dec 27 01:12:29 2026 GMT
  host: agent-manager.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Manager Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agent-manager-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: agent-manager-dev
provider_slug: agent-manager-dev
slug: agent-manager-dev-domain-security
source_filename: agent-manager-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-manager.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 01:12:29 2026 GMT\n  hsts: false\ndomains:\n- domain: agent-manager.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agent-manager-dev/security/agent-manager-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Agent
- Terminal
- OpenSource
- Go
---
