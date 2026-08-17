---
api_specs:
- filename: spekit-openapi.yml
  format: yaml
  label: Spekit API
  slug: spekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:infra+security@spekit.co"
  - 0 iodef "mailto:security@spekit.co"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spekit.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:infra+security@spekit.co"
  - 0 iodef "mailto:security@spekit.co"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spekit.co
  spf: true
hosts:
- cert_expires: Nov 12 05:43:51 2026 GMT
  host: spekit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:41:09 2026 GMT
  host: api.spekit.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:41:09 2026 GMT
  host: mcp.spekit.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: MCP server host, added by hand — the mechanical probe only reads apis.yml baseURL/Website and OpenAPI servers[], and the MCP endpoint lives in mcp/spekit-mcp.yml. Probed 2026-08-14 via HTTPS HEAD + openssl s_client.
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:41:09 2026 GMT
  host: app.spekit.co
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: Web app host, probed 2026-08-14.
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:44:59 2026 GMT
  host: help.spekit.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Zendesk-hosted help center — carries the API and MCP reference documentation. Probed 2026-08-14.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spekit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spekit, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spekit
provider_slug: spekit
slug: spekit-domain-security
source_filename: spekit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spekit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 05:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spekit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.spekit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    MCP server host, added by hand — the mechanical probe only reads apis.yml baseURL/Website\n    and OpenAPI servers[], and the MCP endpoint lives in mcp/spekit-mcp.yml. Probed\n    2026-08-14 via HTTPS HEAD + openssl s_client.\n- host: app.spekit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains:\
  \ false\n  note: Web app host, probed 2026-08-14.\n- host: help.spekit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Zendesk-hosted help center — carries the API and MCP reference documentation. Probed 2026-08-14.\ndomains:\n- domain: spekit.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:infra+security@spekit.co\"\n  - 0 iodef \"mailto:security@spekit.co\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spekit.co\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:infra+security@spekit.co\"\n  - 0 iodef \"mailto:security@spekit.co\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/security/spekit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Saas
- Sales Enablement
- Revenue Enablement
- Digital Adoption
- Knowledge Management
- MCP
- Artificial Intelligence
- Analytics
- Sales
- Content Management
- Agents
- OAuth
---
