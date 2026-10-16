---
api_specs:
- filename: snipe-it-openapi-generated.yml
  format: yaml
  label: Snipe-IT API
  slug: snipe-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipe-it/refs/heads/main/openapi/_ae-authored/snipe-it-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snipeitapp.com
  spf: true
hosts:
- cert_expires: Jan  4 14:04:05 2027 GMT
  host: snipeitapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Snipe It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snipe-IT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snipe-IT
provider_slug: snipe-it
slug: snipe-it-domain-security
source_filename: snipe-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snipeitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 14:04:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snipeitapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snipe-it/refs/heads/main/security/snipe-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IT Asset Management
- Open Source
- Cloud Hosting
- REST API
- Security
- Support
- Software
---
