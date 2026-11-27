---
api_specs:
- filename: dumpthis-sh-agent-api-openapi.yml
  format: yaml
  label: V Tracer Agent API
  slug: dumpthis-sh-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-agent-api-openapi.yml
- filename: dumpthis-sh-lifecycle-api-openapi.yml
  format: yaml
  label: V Tracer Lifecycle API
  slug: dumpthis-sh-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-lifecycle-api-openapi.yml
- filename: dumpthis-sh-mcp-api-openapi.yml
  format: yaml
  label: V Tracer MCP API
  slug: dumpthis-sh-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-mcp-api-openapi.yml
- filename: dumpthis-sh-meta-api-openapi.yml
  format: yaml
  label: V Tracer Meta API
  slug: dumpthis-sh-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-meta-api-openapi.yml
- filename: dumpthis-sh-relay-api-openapi.yml
  format: yaml
  label: V Tracer Relay API
  slug: dumpthis-sh-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-relay-api-openapi.yml
- filename: dumpthis-sh-synack-api-openapi.yml
  format: yaml
  label: V Tracer SYNACK API
  slug: dumpthis-sh-synack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-synack-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dumpthis.sh
  spf: true
hosts:
- cert_expires: Dec  9 22:22:54 2026 GMT
  host: dumpthis.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: V Tracer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for V Tracer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: V Tracer
provider_slug: dumpthis-sh
slug: dumpthis-sh-domain-security
source_filename: dumpthis-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dumpthis.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 22:22:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dumpthis.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dumpthis-sh/security/dumpthis-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Art
- Artificial Intelligence
- Platform
- Open Source
- Experimental
---
