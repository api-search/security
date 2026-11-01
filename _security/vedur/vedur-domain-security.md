---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issuewild "harica.gr"
  - 0 issuewild "globalsign.com"
  - 128 issue "alphassl.com"
  dmarc: false
  dnssec: false
  domain: vedur.is
  spf: true
hosts:
- cert_expires: Apr 17 11:46:04 2027 GMT
  host: vedur.is
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vedur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vedurstofa Islands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vedurstofa Islands
provider_slug: vedur
slug: vedur-domain-security
source_filename: vedur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vedur.is\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 17 11:46:04 2027 GMT\n  hsts: false\ndomains:\n- domain: vedur.is\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issuewild \"globalsign.com\"\n  - 128 issue \"alphassl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/vedur/security/vedur-domain-security.yml
summary_line: TLSv1.2
tags:
- Weather
- Meteorology
- Iceland
- Forecast
- Data
---
