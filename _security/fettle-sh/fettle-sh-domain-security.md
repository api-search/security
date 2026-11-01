---
api_specs:
- filename: fettle-sh-api-openapi.json
  format: json
  label: fettle.sh Api API
  slug: fettle-sh-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fettle-sh/openapi/_original/fettle-sh-api-openapi.json
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
  dmarc_policy: none
  dnssec: true
  domain: fettle.sh
  spf: true
hosts:
- cert_expires: Jan  7 12:38:32 2027 GMT
  host: fettle.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fettle Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fettle-sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: fettle-sh
provider_slug: fettle-sh
slug: fettle-sh-domain-security
source_filename: fettle-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fettle.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 12:38:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fettle.sh\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fettle-sh/security/fettle-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Uptime
- Developers
- AI Agents
- API
---
