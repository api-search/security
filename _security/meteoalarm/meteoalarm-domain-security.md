---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "harica.gr"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:noc@geosphere.at"
  - 0 issue "harica.gr"
  dmarc: false
  dnssec: false
  domain: meteoalarm.org
  spf: true
hosts:
- cert_expires: Jan 13 10:06:56 2027 GMT
  host: meteoalarm.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MeteoAlarm (EUMETNET) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MeteoAlarm (EUMETNET), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MeteoAlarm (EUMETNET)
provider_slug: meteoalarm
slug: meteoalarm-domain-security
source_filename: meteoalarm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meteoalarm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 10:06:56 2027 GMT\n  hsts: false\ndomains:\n- domain: meteoalarm.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:noc@geosphere.at\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/meteoalarm/security/meteoalarm-domain-security.yml
summary_line: TLSv1.3
tags:
- Weather
- EarlyWarning
- Europe
- Public Service
- Meteorology
---
