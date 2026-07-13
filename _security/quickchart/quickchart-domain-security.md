---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: quickchart.io
  spf: true
hosts:
- cert_expires: Oct  2 00:01:57 2026 GMT
  host: quickchart.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quickchart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuickChart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: QuickChart
provider_slug: quickchart
slug: quickchart-domain-security
source_filename: quickchart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickchart.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 00:01:57 2026 GMT\n  hsts: false\ndomains:\n- domain: quickchart.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickchart/refs/heads/main/security/quickchart-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Development
- Public APIs
---
