---
api_specs:
- filename: toptik-app-openapi-generated.yml
  format: yaml
  label: toptik-app API
  slug: toptik-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toptik-app/openapi/_ae-authored/toptik-app-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toptik.app
  spf: true
hosts:
- cert_expires: Jan  7 09:16:49 2027 GMT
  host: toptik.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Toptik App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for toptik-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: toptik-app
provider_slug: toptik-app
slug: toptik-app-domain-security
source_filename: toptik-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toptik.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 09:16:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toptik.app\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/toptik-app/security/toptik-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- TikTok
- Data
- Public
---
