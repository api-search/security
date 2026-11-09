---
api_specs:
- filename: constructionleader-guide-openapi.yml
  format: yaml
  label: Guide Registry API
  slug: guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/constructionleader-guide/openapi/constructionleader-guide-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: constructionleader.guide
  spf: false
hosts:
- cert_expires: Jan  1 12:17:50 2027 GMT
  host: constructionleader.guide
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constructionleader Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Construction Leader Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Construction Leader Guide
provider_slug: constructionleader-guide
slug: constructionleader-guide-domain-security
source_filename: constructionleader-guide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constructionleader.guide\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 12:17:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: constructionleader.guide\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/constructionleader-guide/security/constructionleader-guide-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Construction
- Leadership
- Safety
- Guides
- Bicycle
---
