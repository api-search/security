---
api_specs:
- filename: sweep-api-openapi.yml
  format: yaml
  label: Sweep API
  slug: sweep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/openapi/sweep-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@sweep.io"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sweep.io
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: sweepmcp.com
  note: 'The MCP host runs on a separate registrable domain from sweep.io and inherits none of sweep.io''s posture: no CAA, no DNSSEC, no SPF, no DMARC, and no HSTS header on the OAuth metadata response. sweep.io itself is p=reject with CAA pinning and an iodef security contact.'
  spf: false
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.sweep.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.sweep.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:04:47 2026 GMT
  host: help.sweep.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 13:00:52 2026 GMT
  cert_issuer: Google Trust Services WE1
  edge: cloudflare
  host: sweepmcp.com
  hsts: false
  hsts_max_age: null
  http_version: HTTP/2
  https: true
  note: MCP server host. Probed manually — the mechanical probe only walked *.sweep.io.
  tls_version: TLSv1.3
- host: security.sweep.io
  https: true
  note: HTTP 200, JS-rendered Scytale trust centre.
  role: trust centre
kind: domain-security
layout: security
method: probed
name: Sweep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sweep, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sweep
provider_slug: sweep
slug: sweep-domain-security
source_filename: sweep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sweep.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sweep.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\n- host: help.sweep.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:04:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: sweepmcp.com\n  https: true\n  tls_version: TLSv1.3\n  http_version: HTTP/2\n  cert_expires: Sep 24 13:00:52 2026 GMT\n  cert_issuer: Google Trust Services WE1\n  edge: cloudflare\n  hsts: false\n  hsts_max_age: null\n  note: MCP server host. Probed manually — the mechanical probe only walked *.sweep.io.\n- host: security.sweep.io\n  https: true\n  role: trust centre\n  note: HTTP 200, JS-rendered Scytale trust centre.\ndomains:\n- domain: sweep.io\n  dnssec: false\n\
  \  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@sweep.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sweepmcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  note: 'The MCP host runs on a separate registrable domain from sweep.io and inherits none of sweep.io''s\n    posture: no CAA, no DNSSEC, no SPF, no DMARC, and no HSTS header on the OAuth metadata response. sweep.io\n    itself is p=reject with CAA pinning and an iodef security contact.'\nnotes: Two registrable domains are in play. sweep.io publishes SPF, DMARC p=reject, CAA including iodef\n  mailto:security@sweep.io, and HSTS on www; it does not sign DNSSEC. sweepmcp.com — which serves the\n  OAuth-protected MCP endpoint an agent actually calls — publishes none of these.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/security/sweep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Salesforce
- RevOps
- Metadata
- Governance
- AI Agents
- Model Context Protocol
- Automation
- Documentation
- API
- REST API
- OpenAPI
- Enterprise Systems
- Snowflake
- ServiceNow
- Data Governance
---
