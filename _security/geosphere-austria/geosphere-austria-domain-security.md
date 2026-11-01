---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 iodef "mailto:noc@geosphere.at"
  - 0 issue "sectigo.com"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geosphere.at
  spf: true
hosts:
- cert_expires: Feb  7 09:26:58 2027 GMT
  host: geosphere.at
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geosphere Austria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeoSphere Austria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GeoSphere Austria
provider_slug: geosphere-austria
slug: geosphere-austria-domain-security
source_filename: geosphere-austria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geosphere.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 09:26:58 2027 GMT\n  hsts: false\ndomains:\n- domain: geosphere.at\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:noc@geosphere.at\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geosphere-austria/security/geosphere-austria-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecast
- Austria
- Climate
- Data
- Company
---
