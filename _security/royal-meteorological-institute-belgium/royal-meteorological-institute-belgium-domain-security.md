---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meteo.be
  spf: true
hosts:
- cert_expires: Dec 12 07:32:51 2026 GMT
  host: meteo.be
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Royal Meteorological Institute Belgium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RMI Belgium WOW-BE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RMI Belgium WOW-BE
provider_slug: royal-meteorological-institute-belgium
slug: royal-meteorological-institute-belgium-domain-security
source_filename: royal-meteorological-institute-belgium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meteo.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 07:32:51 2026 GMT\n  hsts: false\ndomains:\n- domain: meteo.be\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/royal-meteorological-institute-belgium/security/royal-meteorological-institute-belgium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Climate
- Meteorology
- Belgium
- PublicSector
---
