---
api_specs:
- filename: accessibe-accounts-api-openapi.yml
  format: yaml
  label: accessiBe Accounts API
  slug: accessibe-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accessibe/refs/heads/main/openapi/accessibe-accounts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accessibe.com
  spf: true
hosts:
- cert_expires: Sep 15 22:41:14 2026 GMT
  host: accessibe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 22:53:42 2026 GMT
  host: dashboard.accessibe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 22:53:42 2026 GMT
  host: flow-mcp.accessibe.com
  hsts: false
  https: true
  note: Cloudflare-fronted; unauthenticated GET / returns 404, POST /mcp returns 401.
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:55:29 2026 GMT
  host: trust.accessibe.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: Third-party hosted trust center (trustcenter.anecdotes.ai).
  tls_version: TLSv1.3
- cert_expires: Oct 24 08:59:03 2026 GMT
  host: status.accessibe.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  note: Third-party hosted status page (statuspage.betteruptime.com).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accessibe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for accessiBe, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: accessiBe
provider_slug: accessibe
slug: accessibe-domain-security
source_filename: accessibe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: The www.npmjs.com host reached via the accessFlow MCP humanURL was excluded —\n  it is a package registry, not an accessiBe-controlled domain.\nhosts:\n- host: accessibe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:41:14 2026 GMT\n  hsts: false\n- host: dashboard.accessibe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:53:42 2026 GMT\n  hsts: false\n- host: flow-mcp.accessibe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:53:42 2026 GMT\n  hsts: false\n  note: Cloudflare-fronted; unauthenticated GET / returns 404, POST /mcp returns 401.\n- host: trust.accessibe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:55:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: Third-party hosted trust center (trustcenter.anecdotes.ai).\n- host: status.accessibe.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Oct 24 08:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  note: Third-party hosted status page (statuspage.betteruptime.com).\ndomains:\n- domain: accessibe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n- No HSTS on the primary website or on the API host (dashboard.accessibe.com).\n- No CAA records published for accessibe.com.\n- DNSSEC is not enabled for accessibe.com.\n- DMARC is published with an enforcing p=reject policy, and SPF is present.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accessibe/refs/heads/main/security/accessibe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accessibility
- Web Accessibility
- WCAG
- ADA Compliance
- Compliance
- Developer Tools
- Testing
- Quality Assurance
- Artificial Intelligence
---
