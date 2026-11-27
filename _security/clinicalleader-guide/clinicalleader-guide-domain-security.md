---
api_specs:
- filename: clinicalleader-guide-openapi.yml
  format: yaml
  label: Bicycle Guide Registry API
  slug: guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clinicalleader-guide/openapi/clinicalleader-guide-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: clinicalleader.guide
  spf: false
hosts:
- cert_expires: Jan  2 09:04:27 2027 GMT
  host: clinicalleader.guide
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clinical Leader Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clinical Leader Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Clinical Leader Guide
provider_slug: clinicalleader-guide
slug: clinicalleader-guide-domain-security
source_filename: clinicalleader-guide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clinicalleader.guide\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 09:04:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clinicalleader.guide\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/clinicalleader-guide/security/clinicalleader-guide-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Clinical Leadership
- Patient Safety
- Healthcare
- Leadership
- Guides
- Publishing
- Education
---
