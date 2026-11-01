---
api_specs:
- filename: stay22-openapi-generated.yml
  format: yaml
  label: Stay22 API
  slug: stay22-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stay22/openapi/_ae-authored/stay22-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stay22.com
  spf: true
hosts:
- cert_expires: Jan 18 01:13:28 2027 GMT
  host: stay22.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stay22 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stay22, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stay22
provider_slug: stay22
slug: stay22-domain-security
source_filename: stay22-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stay22.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 01:13:28 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: stay22.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/stay22/security/stay22-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- TravelTech
- AffiliateMarketing
- SaaS
- Events
- Maps
---
