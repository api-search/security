---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eoddata.com
  spf: true
hosts:
- cert_expires: Jan 27 07:18:06 2027 GMT
  host: eoddata.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EODData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EODData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EODData
provider_slug: eoddata-com
slug: eoddata-com-domain-security
source_filename: eoddata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eoddata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 07:18:06 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: eoddata.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/eoddata-com/security/eoddata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stock Data
- Historical Data
- Intraday Data
- Data Feed
---
