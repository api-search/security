---
api_specs:
- filename: chamelio-openapi-generated.yml
  format: yaml
  label: Chamelio API
  slug: chamelio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chamelio/openapi/_ae-authored/chamelio-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chamelio.ai
  spf: true
hosts:
- cert_expires: Jan  8 15:02:38 2027 GMT
  host: chamelio.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chamelio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chamelio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chamelio
provider_slug: chamelio
slug: chamelio-domain-security
source_filename: chamelio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chamelio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 15:02:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chamelio.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chamelio/security/chamelio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- LegalTech
- SaaS
- Contracts
- Compliance
---
