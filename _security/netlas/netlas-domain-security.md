---
api_specs:
- filename: netlas-openapi-generated.yml
  format: yaml
  label: Netlas API
  slug: netlas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netlas/openapi/_ae-authored/netlas-openapi-generated.yml
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
  dmarc_policy: reject
  dnssec: true
  domain: netlas.io
  spf: true
hosts:
- cert_expires: Jan 13 18:42:31 2027 GMT
  host: netlas.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Netlas
provider_slug: netlas
slug: netlas-domain-security
source_filename: netlas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netlas.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 18:42:31 2027 GMT\n  hsts: false\ndomains:\n- domain: netlas.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/netlas/security/netlas-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Security
- OSINT
- Internet Scanning
- Threat Intelligence
---
