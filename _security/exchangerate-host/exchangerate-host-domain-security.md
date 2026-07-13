---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exchangerate.host
  spf: true
hosts:
- cert_expires: Sep 20 08:32:22 2026 GMT
  host: exchangerate.host
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exchangerate Host Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exchangerate.host, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Exchangerate.host
provider_slug: exchangerate-host
slug: exchangerate-host-domain-security
source_filename: exchangerate-host-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exchangerate.host\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: exchangerate.host\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchangerate-host/refs/heads/main/security/exchangerate-host-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Currency Exchange
- Public APIs
---
