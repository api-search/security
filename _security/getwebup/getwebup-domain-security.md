---
api_specs:
- filename: getwebup-v1-openapi.json
  format: json
  label: Getwebup Cloud API V1 API
  slug: getwebup-cloud-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getwebup/openapi/_original/getwebup-v1-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getwebup.in
  spf: true
hosts:
- cert_expires: Dec 18 23:35:07 2026 GMT
  host: www.getwebup.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getwebup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getwebup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Getwebup
provider_slug: getwebup
slug: getwebup-domain-security
source_filename: getwebup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getwebup.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:35:07 2026 GMT\n  hsts: false\ndomains:\n- domain: getwebup.in\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getwebup/security/getwebup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
