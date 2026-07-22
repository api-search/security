---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vetted.ai
  spf: true
hosts:
- cert_expires: Aug 29 11:15:14 2026 GMT
  host: vetted.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.vetted.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http2: true
  https: true
  note: 'Private app-backend behind Cloudflare. Root returns an 8-byte placeholder; /api-docs and /api/v1 return 403 (auth-gated). No public OpenAPI/Swagger/GraphQL or developer docs are exposed. CORS is wide-open (access-control-allow-origin: *) and auth is header-based (Authorization, X-Session-ID).'
kind: domain-security
layout: security
method: probed
name: Vetted Fka Lustre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vetted (FKA Lustre), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vetted (FKA Lustre)
provider_slug: vetted-fka-lustre
slug: vetted-fka-lustre-domain-security
source_filename: vetted-fka-lustre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + discovered app-backend host\nhosts:\n- host: vetted.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vetted.ai\n  https: true\n  http2: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Private app-backend behind Cloudflare. Root returns an 8-byte placeholder;\n    /api-docs and /api/v1 return 403 (auth-gated). No public OpenAPI/Swagger/GraphQL\n    or developer docs are exposed. CORS is wide-open (access-control-allow-origin: *)\n    and auth is header-based (Authorization, X-Session-ID).\ndomains:\n- domain: vetted.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vetted-fka-lustre/refs/heads/main/security/vetted-fka-lustre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Shopping
- E-commerce
- Consumer
- Product Discovery
- Price Comparison
- Reviews
---
