---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "telesec.de"
  - 0 issuewild "digicert.com"
  - 0 issue "eunetic.de"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bayern.de
  spf: true
hosts:
- cert_expires: Feb  4 23:15:20 2027 GMT
  host: geodaten.bayern.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freistaat Bayern (geodata) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freistaat Bayern (geodata), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Freistaat Bayern (geodata)
provider_slug: bayern-de
slug: bayern-de-domain-security
source_filename: bayern-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geodaten.bayern.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:15:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bayern.de\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"telesec.de\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"eunetic.de\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bayern-de/security/bayern-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Geospatial
- Open Data
- OGC
- WMS
- WFS
- Germany
- Mapping
---
