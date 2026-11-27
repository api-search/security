---
api_specs:
- filename: lotsinvoice-com-openapi-generated.yml
  format: yaml
  label: LotsInvoice API
  slug: lotsinvoice-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotsinvoice-com/openapi/_ae-authored/lotsinvoice-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lotsinvoice.com
  spf: false
hosts:
- cert_expires: Jan  7 08:00:08 2027 GMT
  host: lotsinvoice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LotsInvoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotsInvoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: LotsInvoice
provider_slug: lotsinvoice-com
slug: lotsinvoice-com-domain-security
source_filename: lotsinvoice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lotsinvoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 08:00:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lotsinvoice.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lotsinvoice-com/security/lotsinvoice-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoicing
- Software-as-a-Service
- Small Business
- Freelancers
- Cloud
---
