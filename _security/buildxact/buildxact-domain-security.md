---
api_specs:
- filename: buildxact-public-api-openapi.yml
  format: yaml
  label: Buildxact Public API
  slug: buildxact-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/openapi/buildxact-public-api-openapi.yml
- filename: buildxact-webhooks-asyncapi.yml
  format: yaml
  label: Buildxact Webhooks
  slug: buildxact-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/asyncapi/buildxact-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buildxact.com
  spf: true
hosts:
- cert_expires: Sep 25 14:34:19 2026 GMT
  host: www.buildxact.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: developer.buildxact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.buildxact.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildxact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildxact, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buildxact
provider_slug: buildxact
slug: buildxact-domain-security
source_filename: buildxact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buildxact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:34:19 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: developer.buildxact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.buildxact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buildxact.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/security/buildxact-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Residential Construction
- Construction Management
- Estimating
- Takeoffs
- Job Management
- Project Management
- Quoting
- Scheduling
- Purchase Orders
- Invoicing
- Supplier Integration
- Material Pricing
- Builders
- Remodelers
- Trades
- SaaS
- Australia
- Autodesk
---
