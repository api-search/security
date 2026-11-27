---
api_specs:
- filename: govauctions-app-openapi-generated.yml
  format: yaml
  label: Gov Auctions API
  slug: govauctions-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govauctions-app/openapi/_ae-authored/govauctions-app-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:dmarc@govauctions.app"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: govauctions.app
  spf: true
hosts:
- cert_expires: Jan 12 22:32:33 2027 GMT
  host: govauctions.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gov Auctions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gov Auctions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gov Auctions
provider_slug: govauctions-app
slug: govauctions-app-domain-security
source_filename: govauctions-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govauctions.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 22:32:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: govauctions.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:dmarc@govauctions.app\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/govauctions-app/security/govauctions-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auctions
- Government
- Surplus
- Marketplace
- Search
---
