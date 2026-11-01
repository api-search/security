---
api_specs:
- filename: ansvar-eu-openapi-generated.yml
  format: yaml
  label: ansvar-eu API
  slug: ansvar-eu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ansvar-eu/openapi/_ae-authored/ansvar-eu-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ansvar.eu
  spf: true
hosts:
- cert_expires: Dec 11 03:21:19 2026 GMT
  host: ansvar.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ansvar Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ansvar-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ansvar-eu
provider_slug: ansvar-eu
slug: ansvar-eu-domain-security
source_filename: ansvar-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ansvar.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 03:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ansvar.eu\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ansvar-eu/security/ansvar-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Compliance
- Legal
- Security
- Data
---
