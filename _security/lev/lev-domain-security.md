---
api_specs:
- filename: lev-openapi-original.json
  format: json
  label: Lev API
  slug: lev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lev/refs/heads/main/openapi/lev-openapi-original.json
description: ''
domains:
- caa: []
  caa_note: Re-queried against 8.8.8.8 on 2026-07-19 — the zone genuinely publishes no CAA records. (An earlier probe pass recorded a resolver timeout here; that was a lookup artifact, not a record.)
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lev.com
  spf: true
hosts:
- cert_expires: Aug 28 12:15:05 2026 GMT
  host: www.lev.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.lev.com
  hsts: false
  https: true
  note: No Strict-Transport-Security header observed on the API host, though the marketing/docs host sets one with a one-year max-age. The Lev security docs state HSTS is enforced.
  tls_version: TLSv1.2
- host: mcp.lev.com
  hsts: false
  https: true
  role: hosted MCP server
kind: domain-security
layout: security
method: probed
name: Lev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lev, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lev
provider_slug: lev
slug: lev-domain-security
source_filename: lev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:15:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lev.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n  note: No Strict-Transport-Security header observed on the API host, though the\n    marketing/docs host sets one with a one-year max-age. The Lev security docs\n    state HSTS is enforced.\n- host: mcp.lev.com\n  https: true\n  hsts: false\n  role: hosted MCP server\ndomains:\n- domain: lev.com\n  dnssec: false\n  caa: []\n  caa_note: Re-queried against 8.8.8.8 on 2026-07-19 — the zone genuinely publishes\n    no CAA records. (An earlier probe pass recorded a resolver timeout here; that\n    was a lookup artifact, not a record.)\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n- severity: info\n\
  \  finding: Strong email posture — SPF present and DMARC at policy `reject`.\n- severity: low\n  finding: No DNSSEC on lev.com.\n- severity: low\n  finding: No CAA records, so certificate issuance is not restricted to named CAs.\n- severity: low\n  finding: HSTS is set on www.lev.com but not observed on api.lev.com or\n    mcp.lev.com — the two hosts that carry bearer tokens.\n- severity: info\n  finding: api.lev.com negotiated TLSv1.2 while www.lev.com negotiated TLSv1.3.\n    Both meet the documented TLS 1.2+ floor.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lev/refs/heads/main/security/lev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commercial Real Estate
- Real Estate
- Proptech
- CRE Financing
- Lending
- CRM
- Artificial Intelligence
- AI Agents
- Deal Management
- Market Data
- Documents
---
