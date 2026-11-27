---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: delilahusa.com
  spf: false
hosts:
- cert_expires: Jan 12 02:48:53 2027 GMT
  host: delilahusa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Delilah Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delilah, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Delilah
provider_slug: delilahusa-com
slug: delilahusa-com-domain-security
source_filename: delilahusa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delilahusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 02:48:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: delilahusa.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/delilahusa-com/security/delilahusa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Legislation
- Government
- Civic Technology
- Artificial Intelligence
- Policy
- MCP
- Public Data
---
