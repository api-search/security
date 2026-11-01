---
api_specs:
- filename: brightedge-auth-api-openapi.yml
  format: yaml
  label: BrightEdge Auth API
  slug: brightedge-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-auth-api-openapi.yml
- filename: brightedge-authorize-api-openapi.yml
  format: yaml
  label: BrightEdge Authorize API
  slug: brightedge-authorize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-authorize-api-openapi.yml
- filename: brightedge-feedback-api-openapi.yml
  format: yaml
  label: BrightEdge Feedback API
  slug: brightedge-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-feedback-api-openapi.yml
- filename: brightedge-oauth-api-openapi.yml
  format: yaml
  label: BrightEdge OAuth API
  slug: brightedge-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-oauth-api-openapi.yml
- filename: brightedge-ping-api-openapi.yml
  format: yaml
  label: BrightEdge Ping API
  slug: brightedge-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-ping-api-openapi.yml
- filename: brightedge-saml-api-openapi.yml
  format: yaml
  label: BrightEdge SAML API
  slug: brightedge-saml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-saml-api-openapi.yml
- filename: brightedge-sso-api-openapi.yml
  format: yaml
  label: BrightEdge SSO API
  slug: brightedge-sso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-sso-api-openapi.yml
- filename: brightedge-token-api-openapi.yml
  format: yaml
  label: BrightEdge Token API
  slug: brightedge-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-token-api-openapi.yml
- filename: brightedge-well-known-api-openapi.yml
  format: yaml
  label: BrightEdge .well Known API
  slug: brightedge-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightedge/openapi/brightedge-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  caa_evidence: no CAA record published
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_reporting: dmarcian
  dnssec: false
  dnssec_evidence: no DS record at the parent
  domain: brightedge.com
  spf: true
  spf_record: v=spf1 mx include:amazonses.com include:_spf.google.com include:mail.zendesk.com include:mailsenders.netsuite.com ip4:168.245.58.37 ip4:66.103.215.2 include:spf.protection.outlook.com ~all
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.brightedge.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.brightedge.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: false
  http_status: 302
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: mcp2.brightedge.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 404
  https: true
  role: MCP server (HTTP/streamable)
  tls_version: TLSv1.3
- host: mcp.brightedge.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 404
  https: true
  role: MCP endpoint behind the OpenAI plugin marketplace
  tls_version: TLSv1.3
- host: mcp2-sse.brightedge.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 401
  https: true
  role: MCP server (SSE)
  tls_version: TLSv1.3
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Brightedge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrightEdge, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BrightEdge
provider_slug: brightedge
slug: brightedge-domain-security
source_filename: brightedge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI + MCP hosts\nnote: >-\n  Header values read with a browser User-Agent. The mechanical probe returns hsts:null and\n  dmarc:false against these hosts because api.brightedge.com and the MCP hosts reject the default\n  probe client — the values below are the observed response headers and the live DNS records, not\n  the probe's false negatives.\nhosts:\n- host: www.brightedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  http_status: 200\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: api.brightedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  http_status: 302\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: false\n- host: mcp2.brightedge.com\n  role: MCP server (HTTP/streamable)\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  http_status: 404\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: mcp.brightedge.com\n  role: MCP endpoint behind the OpenAI plugin marketplace\n  https: true\n  tls_version: TLSv1.3\n  http_status: 404\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: mcp2-sse.brightedge.com\n  role: MCP server (SSE)\n  https: true\n  tls_version: TLSv1.3\n  http_status: 401\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: brightedge.com\n  dnssec: false\n  dnssec_evidence: no DS record at the parent\n  caa: []\n  caa_evidence: no CAA record published\n  spf: true\n  spf_record: v=spf1 mx include:amazonses.com include:_spf.google.com include:mail.zendesk.com\n    include:mailsenders.netsuite.com ip4:168.245.58.37 ip4:66.103.215.2 include:spf.protection.outlook.com\n    ~all\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 100\n  dmarc_reporting: dmarcian\nresponse_headers_observed:\n  mcp2.brightedge.com:\n    x-content-type-options: nosniff\n    content-security-policy: default-src 'self' frame-ancestors 'self'\n    referrer-policy: strict-origin-when-cross-origin\n    permissions-policy: geolocation=(), camera=(), microphone=()\n    server: Google Frontend\n"
source_yaml_url: https://artifacts.apis.io/brightedge/security/brightedge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SEO
- Search
- Content
- Marketing
- Analytics
- Keywords
- Enterprise
- AI Search
---
