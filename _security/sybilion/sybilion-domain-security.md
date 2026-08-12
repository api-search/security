---
api_specs:
- filename: sybilion-operational-api-openapi.yml
  format: yaml
  label: Sybilion Operational API
  slug: sybilion-operational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-operational-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: sybilion.dev
  ds_record: false
  role: product domain (API, MCP, docs, portal)
  spf: false
  txt_records_present:
  - google-site-verification
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:<redacted>@dmarc-reports.cloudflare.net;
  dnssec: false
  domain: sybilion.com
  ds_record: false
  note: DMARC is at p=quarantine with Cloudflare aggregate reporting, but there is NO v=spf1 record on the apex, so DMARC can only pass via DKIM alignment. support@sybilion.com is the published support and security-report address, which makes the missing SPF record worth flagging.
  role: corporate domain (website, email, Auth0 custom domain)
  spf: false
  txt_records_present:
  - MS=
  - google-site-verification x2
  - anthropic-domain-verification
  - kok6w5nrvl
hosts:
- cert_expires: Nov  4 11:00:55 2026 GMT
  host: sybilion.dev
  hsts: false
  https: true
  role: developer portal (SPA)
  tls_version: TLSv1.3
- cert_expires: Nov  4 11:00:55 2026 GMT
  host: api.sybilion.dev
  hsts: false
  hsts_observed: no strict-transport-security header on 401 /api/v1/me or 405 /health, 2026-08-11
  https: true
  role: REST API
  tls_version: TLSv1.3
- cert_expires: Nov  4 11:00:55 2026 GMT
  host: mcp.sybilion.dev
  hsts: false
  hsts_observed: no strict-transport-security header on the 401 tools/list challenge, 2026-08-11
  https: true
  role: hosted MCP server
  tls_version: TLSv1.3
- cert_expires: Oct  8 13:09:26 2026 GMT
  host: www.sybilion.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: https://sybilion.com/ redirects to https://www.sybilion.com/ (200)
  role: corporate / marketing site (Webflow behind Cloudflare)
  tls_version: TLSv1.3
- host: auth0.sybilion.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: Auth0 custom domain — portal login and MCP OAuth issuer
kind: domain-security
layout: security
method: probed
name: Sybilion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sybilion, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sybilion
provider_slug: sybilion
slug: sybilion-domain-security
source_filename: sybilion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Baseline written by 0-working/probe-domain-security.py (sybilion.dev tree only), then extended by\n  hand with the sybilion.com corporate/marketing domain, the auth0.sybilion.com identity host, and\n  observed HSTS headers — none of which are reachable from apis.yml as it stood. Headline: TLS 1.3\n  everywhere and HSTS on the two Cloudflare-fronted web properties, but the API and MCP hosts return\n  NO HSTS header at all, and neither registrable domain has DNSSEC, CAA, or SPF. sybilion.dev — the\n  domain that serves the API, the MCP server and the developer portal — has no DMARC record either.\nhosts:\n- host: sybilion.dev\n  role: developer portal (SPA)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:00:55 2026 GMT\n  hsts: false\n- host: api.sybilion.dev\n  role: REST API\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:00:55\
  \ 2026 GMT\n  hsts: false\n  hsts_observed: 'no strict-transport-security header on 401 /api/v1/me or 405 /health, 2026-08-11'\n- host: mcp.sybilion.dev\n  role: hosted MCP server\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:00:55 2026 GMT\n  hsts: false\n  hsts_observed: 'no strict-transport-security header on the 401 tools/list challenge, 2026-08-11'\n- host: www.sybilion.com\n  role: corporate / marketing site (Webflow behind Cloudflare)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:09:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  note: 'https://sybilion.com/ redirects to https://www.sybilion.com/ (200)'\n- host: auth0.sybilion.com\n  role: Auth0 custom domain — portal login and MCP OAuth issuer\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: sybilion.dev\n  role: product domain (API, MCP, docs, portal)\n  dnssec: false\n  ds_record: false\n\
  \  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  txt_records_present: [google-site-verification]\n- domain: sybilion.com\n  role: corporate domain (website, email, Auth0 custom domain)\n  dnssec: false\n  ds_record: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; rua=mailto:<redacted>@dmarc-reports.cloudflare.net;'\n  txt_records_present: [MS=, google-site-verification x2, anthropic-domain-verification, kok6w5nrvl]\n  note: >-\n    DMARC is at p=quarantine with Cloudflare aggregate reporting, but there is NO v=spf1 record on\n    the apex, so DMARC can only pass via DKIM alignment. support@sybilion.com is the published\n    support and security-report address, which makes the missing SPF record worth flagging.\nfindings:\n  - { severity: low, item: 'no CAA records on either domain — any CA may issue' }\n  - { severity: low, item: 'no DNSSEC on either domain' }\n  - { severity: medium, item: 'no HSTS on\
  \ api.sybilion.dev or mcp.sybilion.dev, the two credential-bearing hosts' }\n  - { severity: medium, item: 'no SPF on sybilion.com despite DMARC p=quarantine' }\n  - { severity: medium, item: 'no DMARC at all on sybilion.dev' }\n  - { severity: info, item: 'TLS 1.3 on every host; certificates valid through Oct/Nov 2026' }\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/security/sybilion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial market intelligence
- Commodity price forecasting
- Economic forecasting
- Time-series forecasting
- Procurement
- Supply-chain risk
- Trading analytics
- AI decision support
- MCP
- Agent-native
- Causal inference
- Anomaly detection
---
