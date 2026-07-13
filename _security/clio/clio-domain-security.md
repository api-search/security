---
api_specs:
- filename: clio-manage-api-v4-openapi.yml
  format: yaml
  label: Clio Manage API v4
  slug: manage-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clio/refs/heads/main/openapi/clio-manage-api-v4-openapi.yml
- filename: clio-webhooks-asyncapi.yml
  format: yaml
  label: Clio Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/clio/refs/heads/main/asyncapi/clio-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clio.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.clio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: docs.developers.clio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: app.clio.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clio
provider_slug: clio
slug: clio-domain-security
source_filename: clio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.developers.clio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n- host: app.clio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: clio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clio/refs/heads/main/security/clio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Calendaring
- Document Management
- Law Firms
- Legal
- Matter Management
- OAuth 2.0
- Practice Management
- Time Tracking
- Trust Accounting
---
