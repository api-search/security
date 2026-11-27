---
api_specs:
- filename: alto-video-openapi-generated.yml
  format: yaml
  label: Alto API
  slug: alto-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alto-video/openapi/_ae-authored/alto-video-openapi-generated.yml
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
  dmarc_policy: none
  dnssec: false
  domain: alto.video
  spf: true
hosts:
- cert_expires: Dec 12 19:46:06 2026 GMT
  host: alto.video
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alto
provider_slug: alto-video
slug: alto-video-domain-security
source_filename: alto-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alto.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 19:46:06 2026 GMT\n  hsts: false\ndomains:\n- domain: alto.video\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/alto-video/security/alto-video-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video Hosting
- Sales Enablement
- Demo Analytics
- Privacy
- Software-as-a-Service
---
