---
api_specs:
- filename: dejavoo-openapi-generated.yml
  format: yaml
  label: Dejavoo API
  slug: dejavoo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dejavoo/openapi/_ae-authored/dejavoo-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dejavoo.io
  spf: true
hosts:
- cert_expires: Jan 31 18:31:07 2027 GMT
  host: dejavoo.io
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dejavoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dejavoo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dejavoo
provider_slug: dejavoo
slug: dejavoo-domain-security
source_filename: dejavoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dejavoo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 18:31:07 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: dejavoo.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dejavoo/security/dejavoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Payment Terminals
- Point-of-Sale
- Payment Gateway
- Semi-Integration
- Fintech
- Merchant Services
---
