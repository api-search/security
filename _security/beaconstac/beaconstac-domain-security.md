---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Uniqode QR Code API
  slug: uniqode-qr-code-api
  spec_type: Postman
  url: https://apidocs.uniqode.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uniqode.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.uniqode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 03:47:52 2026 GMT
  host: apidocs.uniqode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.uniqode.com
  hsts: null
  https: true
  note: The API host is the ONLY Uniqode host probed that serves no HSTS and still negotiates TLS 1.2 as its top protocol — weaker than the marketing, docs, dashboard and identity hosts, all of which reach TLS 1.3.
  tls_version: TLSv1.2
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: mcp.uniqode.com
  hsts: false
  https: true
  role: hosted MCP server (uvicorn), OAuth-protected
  tls_version: TLSv1.2
- cert_expires: Sep 26 15:24:09 2026 GMT
  host: auth.uniqode.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: OAuth 2.0 / OIDC authorization server (Auth0 custom domain)
  tls_version: TLSv1.3
- cert_expires: Oct 22 00:06:44 2026 GMT
  host: dashboard.uniqode.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  role: application dashboard (Angular SPA)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beaconstac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beaconstac, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Beaconstac
provider_slug: beaconstac
slug: beaconstac-domain-security
source_filename: beaconstac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (+ the MCP/identity hosts found in round 2)\nhosts:\n- host: www.uniqode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.uniqode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 03:47:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uniqode.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n  note: >-\n    The API host is the ONLY Uniqode host probed that serves no HSTS and still negotiates\n    TLS 1.2 as its top protocol — weaker than the marketing, docs, dashboard and identity hosts,\n    all of which reach TLS 1.3.\n- host: mcp.uniqode.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n  role: hosted MCP server (uvicorn), OAuth-protected\n- host:\
  \ auth.uniqode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  role: OAuth 2.0 / OIDC authorization server (Auth0 custom domain)\n- host: dashboard.uniqode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 00:06:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n  role: application dashboard (Angular SPA)\ndomains:\n- domain: uniqode.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconstac/refs/heads/main/security/beaconstac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Big Data
- QR Codes
- Digital Business Cards
- Marketing
- Analytics
- SaaS
- Proximity
- Webhooks
- MCP
---
