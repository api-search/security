---
api_specs:
- filename: magic-link-openapi.yml
  format: yaml
  label: Magic Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-link/refs/heads/main/openapi/magic-link-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: magic.link
  spf: true
hosts:
- cert_expires: Aug 14 14:52:50 2026 GMT
  host: magic.link
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 19:32:21 2026 GMT
  host: api.magic.link
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 17:12:17 2026 GMT
  host: api.toaster.magic.link
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Link Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Magic
provider_slug: magic-link
slug: magic-link-domain-security
source_filename: magic-link-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magic.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 14:52:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.magic.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:32:21 2026 GMT\n  hsts: null\n- host: api.toaster.magic.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:12:17 2026 GMT\n  hsts: null\ndomains:\n- domain: magic.link\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-link/refs/heads/main/security/magic-link-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
