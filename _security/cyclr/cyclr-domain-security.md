---
api_specs:
- filename: cyclr-cyclr-openapi.yml
  format: yaml
  label: Cyclr API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/openapi/cyclr-cyclr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cyclr.com
  spf: true
hosts:
- cert_expires: Sep  5 07:10:57 2026 GMT
  host: cyclr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.cyclr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.eu.cyclr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cyclr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyclr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cyclr
provider_slug: cyclr
slug: cyclr-domain-security
source_filename: cyclr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyclr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:10:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cyclr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.eu.cyclr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cyclr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/security/cyclr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integrations
- Marketplace
- OAuth 2.0
- REST API
- SaaS
- Templates
- Webhooks
- White Label
- Workflows
---
