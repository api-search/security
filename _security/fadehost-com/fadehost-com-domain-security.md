---
api_specs:
- filename: fadehost-com-openapi-generated.yml
  format: yaml
  label: FadeHost API
  slug: fadehost-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fadehost-com/openapi/_ae-authored/fadehost-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fadehost.com
  spf: true
hosts:
- cert_expires: Jan  1 22:12:17 2027 GMT
  host: fadehost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FadeHost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FadeHost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FadeHost
provider_slug: fadehost-com
slug: fadehost-com-domain-security
source_filename: fadehost-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fadehost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 22:12:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fadehost.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fadehost-com/security/fadehost-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hosting
- Gaming
- Minecraft
- Cloud
---
