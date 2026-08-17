---
api_specs:
- filename: northbeam-orders-v2-openapi.yml
  format: yaml
  label: Northbeam Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/openapi/northbeam-orders-v2-openapi.yml
- filename: northbeam-spend-v1-openapi.yml
  format: yaml
  label: Northbeam Spend API
  slug: spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/openapi/northbeam-spend-v1-openapi.yml
- filename: northbeam-data-export-v1-openapi.yml
  format: yaml
  label: Northbeam Data Export API
  slug: data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/openapi/northbeam-data-export-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: northbeam.io
  spf: true
hosts:
- cert_expires: Oct  1 02:03:36 2026 GMT
  host: www.northbeam.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 01:13:38 2026 GMT
  host: docs.northbeam.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 11:33:49 2026 GMT
  host: api.northbeam.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- added_by: enrichment pass 2026-08-13 (host is not in the OpenAPI servers[] the script reads)
  cert_expires: Nov  5 17:34:40 2026 GMT
  host: mcp.northbeam.io
  hsts: null
  https: true
  note: agent surface; returns 401 with a WWW-Authenticate Bearer challenge on every path
- added_by: enrichment pass 2026-08-13 (host is not in the OpenAPI servers[] the script reads)
  cert_expires: Sep 27 05:25:07 2026 GMT
  host: auth.northbeam.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Auth0 identity tenant backing the MCP OAuth flow
- added_by: enrichment pass 2026-08-13
  cert_expires: Oct 29 21:18:18 2026 GMT
  host: api-uat.northbeam.io
  hsts: null
  https: true
  note: UAT sandbox host declared in the Orders and Spend servers[] blocks
kind: domain-security
layout: security
method: probed
name: Northbeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northbeam, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Northbeam
provider_slug: northbeam
slug: northbeam-domain-security
source_filename: northbeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.northbeam.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.northbeam.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 01:13:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.northbeam.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:33:49 2026 GMT\n  hsts: null\n- host: mcp.northbeam.io\n  https: true\n  cert_expires: Nov  5 17:34:40 2026 GMT\n  hsts: null\n  note: agent surface; returns 401 with a WWW-Authenticate Bearer challenge on every path\n  added_by: enrichment pass 2026-08-13 (host is not in the OpenAPI servers[] the script reads)\n- host: auth.northbeam.io\n  https: true\n  cert_expires: Sep 27 05:25:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Auth0 identity\
  \ tenant backing the MCP OAuth flow\n  added_by: enrichment pass 2026-08-13 (host is not in the OpenAPI servers[] the script reads)\n- host: api-uat.northbeam.io\n  https: true\n  cert_expires: Oct 29 21:18:18 2026 GMT\n  hsts: null\n  note: UAT sandbox host declared in the Orders and Spend servers[] blocks\n  added_by: enrichment pass 2026-08-13\nx-hsts-gap: >\n  HSTS is served on www.northbeam.io, docs.northbeam.io and auth.northbeam.io but NOT on\n  api.northbeam.io, api-uat.northbeam.io or mcp.northbeam.io — the three hosts that actually\n  carry API credentials.\ndomains:\n- domain: northbeam.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/security/northbeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketing Attribution
- Multi-Touch Attribution
- E-Commerce
- ROAS
- Media Mix Modeling
- Creative Analytics
- Performance Marketing
- Advertising
- Marketing Analytics
- Agents
---
