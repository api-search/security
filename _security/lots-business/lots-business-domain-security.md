---
api_specs:
- filename: lots-business-openapi-generated.yml
  format: yaml
  label: LotsBusiness API
  slug: lots-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-business/openapi/_ae-authored/lots-business-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lots.business
  spf: false
hosts:
- cert_expires: Jan  7 16:15:33 2027 GMT
  host: lots.business
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LotsBusiness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotsBusiness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: LotsBusiness
provider_slug: lots-business
slug: lots-business-domain-security
source_filename: lots-business-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lots.business\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:15:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lots.business\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lots-business/security/lots-business-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business
- Websites
- Artificial Intelligence
- Email
- Branding
---
