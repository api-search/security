---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: manuotel.com
  spf: false
hosts:
- cert_expires: Jan 25 03:46:33 2027 GMT
  host: manuotel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Manu Otel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manu Otel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Manu Otel
provider_slug: manuotel-com
slug: manuotel-com-domain-security
source_filename: manuotel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manuotel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 03:46:33 2027 GMT\n  hsts: false\ndomains:\n- domain: manuotel.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/manuotel-com/security/manuotel-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Artificial Intelligence
- LLM
- Agents
- Open Source
---
