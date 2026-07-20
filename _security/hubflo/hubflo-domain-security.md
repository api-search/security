---
api_specs:
- filename: hubflo-openapi-original.yml
  format: yaml
  label: Hubflo API
  slug: hubflo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubflo/refs/heads/main/openapi/hubflo-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hubflo.com
  spf: true
hosts:
- cert_expires: Sep 15 03:55:19 2026 GMT
  host: hubflo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- host: app.hubflo.com
  https: false
- host: staging.hubflo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hubflo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hubflo, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hubflo
provider_slug: hubflo
slug: hubflo-domain-security
source_filename: hubflo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hubflo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 03:55:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.hubflo.com\n  https: false\n- host: staging.hubflo.com\n  https: false\ndomains:\n- domain: hubflo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubflo/refs/heads/main/security/hubflo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Client Portal
- Professional Services
- CRM
- Invoicing
- Project Management
- Document Management
- E-Signature
- Onboarding
- Webhooks
- Company
---
