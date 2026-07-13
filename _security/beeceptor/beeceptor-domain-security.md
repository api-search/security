---
api_specs:
- filename: beeceptor-openapi.yml
  format: yaml
  label: Beeceptor API
  slug: beeceptor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeceptor/refs/heads/main/openapi/beeceptor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beeceptor.com
  spf: true
hosts:
- cert_expires: Sep 12 08:09:58 2026 GMT
  host: beeceptor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: app.beeceptor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 10:37:56 2026 GMT
  host: api.beeceptor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beeceptor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beeceptor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beeceptor
provider_slug: beeceptor
slug: beeceptor-domain-security
source_filename: beeceptor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beeceptor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:09:58 2026 GMT\n  hsts: false\n- host: app.beeceptor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.beeceptor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:37:56 2026 GMT\n  hsts: null\ndomains:\n- domain: beeceptor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeceptor/refs/heads/main/security/beeceptor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Mocking
- Automation
- Debugging
- HTTP Proxy
- Integrations
- Mock Servers
- Platform
- Testing
- Webhooks
---
