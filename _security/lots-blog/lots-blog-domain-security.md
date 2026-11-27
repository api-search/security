---
api_specs:
- filename: lots-blog-lots-blog-api-openapi.yml
  format: yaml
  label: LotsBlog Lots.Blog API
  slug: lots-blog-lots-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-blog/openapi/lots-blog-lots-blog-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lots.blog
  spf: false
hosts:
- cert_expires: Jan  7 08:09:01 2027 GMT
  host: lots.blog
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LotsBlog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotsBlog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: LotsBlog
provider_slug: lots-blog
slug: lots-blog-domain-security
source_filename: lots-blog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lots.blog\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 08:09:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lots.blog\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lots-blog/security/lots-blog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Blogging
- Content Creation
- Automation
---
