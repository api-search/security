---
api_specs:
- filename: deerdawn-com-auth-api-openapi.yml
  format: yaml
  label: DeerDawn Auth API
  slug: deerdawn-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-auth-api-openapi.yml
- filename: deerdawn-com-keys-api-openapi.yml
  format: yaml
  label: DeerDawn Keys API
  slug: deerdawn-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-keys-api-openapi.yml
- filename: deerdawn-com-session-memory-api-openapi.yml
  format: yaml
  label: DeerDawn Session Memory API
  slug: deerdawn-com-session-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-session-memory-api-openapi.yml
- filename: deerdawn-com-system-api-openapi.yml
  format: yaml
  label: DeerDawn System API
  slug: deerdawn-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deerdawn-com/openapi/deerdawn-com-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: deerdawn.com
  spf: true
hosts:
- cert_expires: Jan 28 16:02:47 2027 GMT
  host: deerdawn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DeerDawn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeerDawn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DeerDawn
provider_slug: deerdawn-com
slug: deerdawn-com-domain-security
source_filename: deerdawn-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deerdawn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:02:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deerdawn.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deerdawn-com/security/deerdawn-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Session Memory
- MCP
- Productivity
- Platform
- Company
---
