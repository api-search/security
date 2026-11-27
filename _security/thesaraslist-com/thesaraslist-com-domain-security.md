---
api_specs:
- filename: thesaraslist-com-v1-openapi.json
  format: json
  label: Sara's List API V1 API
  slug: sara-s-list-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thesaraslist-com/openapi/_original/thesaraslist-com-v1-openapi.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: thesaraslist.com
  spf: true
hosts:
- cert_expires: Dec 31 12:24:22 2026 GMT
  host: thesaraslist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sara's List Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sara''s List, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sara's List
provider_slug: thesaraslist-com
slug: thesaraslist-com-domain-security
source_filename: thesaraslist-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesaraslist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 12:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thesaraslist.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/thesaraslist-com/security/thesaraslist-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job Board
- Startup Jobs
- Equity Compensation
- Remote Jobs
- Growth‑stage Companies
---
