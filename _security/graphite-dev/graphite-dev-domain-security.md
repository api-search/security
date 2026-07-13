---
api_specs:
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite GitHub App
  slug: graphite-github-app
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite CLI (gt)
  slug: graphite-cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite GT MCP Server
  slug: graphite-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Agent (Diamond) AI Code Review
  slug: graphite-agent-diamond
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Merge Queue
  slug: graphite-merge-queue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Insights
  slug: graphite-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graphite.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graphite.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: graphite.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: graphite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: app.graphite.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphite Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphite, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Graphite
provider_slug: graphite-dev
slug: graphite-dev-domain-security
source_filename: graphite-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphite.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: graphite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.graphite.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: graphite.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: graphite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/security/graphite-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub
---
