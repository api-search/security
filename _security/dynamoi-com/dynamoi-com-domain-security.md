---
api_specs:
- filename: dynamoi-com-data-api-openapi.yml
  format: yaml
  label: Dynamoi Data API
  slug: dynamoi-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamoi-com/openapi/dynamoi-com-data-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dynamoi.com
  spf: true
hosts:
- cert_expires: Jan 23 01:46:59 2027 GMT
  host: dynamoi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynamoi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamoi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dynamoi
provider_slug: dynamoi-com
slug: dynamoi-com-domain-security
source_filename: dynamoi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynamoi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 01:46:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dynamoi.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dynamoi-com/security/dynamoi-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Music Promotion
- Spotify
- YouTube
- Distribution
- Analytics
- Independent Artists
- Labels
---
