---
api_specs:
- filename: nango-openapi.yml
  format: yaml
  label: Nango
  slug: nango
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nango/refs/heads/main/openapi/nango-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nango.dev
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: app.nango.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.nango.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.nango.dev
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nango Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nango, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nango
provider_slug: nango
slug: nango-domain-security
source_filename: nango-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.nango.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.nango.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.nango.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: nango.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nango/refs/heads/main/security/nango-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Integrations
- OAuth
- Syncing
- Unified API
- Webhooks
---
