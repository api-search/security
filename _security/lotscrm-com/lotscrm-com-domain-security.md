---
api_specs:
- filename: lotscrm-com-openapi-generated.yml
  format: yaml
  label: LotsCRM API
  slug: lotscrm-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotscrm-com/openapi/_ae-authored/lotscrm-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lotscrm.com
  spf: false
hosts:
- cert_expires: Jan  7 10:08:15 2027 GMT
  host: lotscrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LotsCRM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotsCRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: LotsCRM
provider_slug: lotscrm-com
slug: lotscrm-com-domain-security
source_filename: lotscrm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lotscrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:08:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lotscrm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lotscrm-com/security/lotscrm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Software-as-a-Service
- Artificial Intelligence
- Sales
- Small Teams
---
