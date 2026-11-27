---
api_specs:
- filename: heyclau-de-admin-api-openapi.yml
  format: yaml
  label: HeyClaude Admin API
  slug: heyclau-de-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-admin-api-openapi.yml
- filename: heyclau-de-commercial-api-openapi.yml
  format: yaml
  label: HeyClaude Commercial API
  slug: heyclau-de-commercial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-commercial-api-openapi.yml
- filename: heyclau-de-distribution-api-openapi.yml
  format: yaml
  label: HeyClaude Distribution API
  slug: heyclau-de-distribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-distribution-api-openapi.yml
- filename: heyclau-de-dynamic-api-openapi.yml
  format: yaml
  label: HeyClaude Dynamic API
  slug: heyclau-de-dynamic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-dynamic-api-openapi.yml
- filename: heyclau-de-jobs-api-openapi.yml
  format: yaml
  label: HeyClaude Jobs API
  slug: heyclau-de-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-jobs-api-openapi.yml
- filename: heyclau-de-mcp-api-openapi.yml
  format: yaml
  label: HeyClaude MCP API
  slug: heyclau-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-mcp-api-openapi.yml
- filename: heyclau-de-newsletter-api-openapi.yml
  format: yaml
  label: HeyClaude Newsletter API
  slug: heyclau-de-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-newsletter-api-openapi.yml
- filename: heyclau-de-registry-api-openapi.yml
  format: yaml
  label: HeyClaude Registry API
  slug: heyclau-de-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-registry-api-openapi.yml
- filename: heyclau-de-submissions-api-openapi.yml
  format: yaml
  label: HeyClaude Submissions API
  slug: heyclau-de-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyclau-de/openapi/heyclau-de-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: heyclau.de
  spf: true
hosts:
- cert_expires: Feb  2 22:52:08 2027 GMT
  host: heyclau.de
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HeyClaude Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeyClaude, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HeyClaude
provider_slug: heyclau-de
slug: heyclau-de-domain-security
source_filename: heyclau-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heyclau.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 22:52:08 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: heyclau.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/heyclau-de/security/heyclau-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Directory
- Claude
- Artificial Intelligence
- Community
- Open Source
- Tools
---
