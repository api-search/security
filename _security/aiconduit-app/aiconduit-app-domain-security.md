---
api_specs:
- filename: aiconduit-app-openapi-generated.yml
  format: yaml
  label: Conduit API
  slug: aiconduit-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiconduit-app/openapi/_ae-authored/aiconduit-app-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: aiconduit.app
  spf: false
hosts:
- cert_expires: Jan 28 05:19:01 2027 GMT
  host: aiconduit.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiconduit App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conduit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Conduit
provider_slug: aiconduit-app
slug: aiconduit-app-domain-security
source_filename: aiconduit-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiconduit.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 05:19:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aiconduit.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aiconduit-app/security/aiconduit-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Procurement
- B2B
- Automation
- Marketplace
- Artificial Intelligence
---
