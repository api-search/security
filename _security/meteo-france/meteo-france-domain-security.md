---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: meteofrance.com
  spf: false
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: meteofrance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meteo France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meteo-France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Meteo-France
provider_slug: meteo-france
slug: meteo-france-domain-security
source_filename: meteo-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meteofrance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: meteofrance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/meteo-france/security/meteo-france-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Weather
- Climate
- Forecast
- Public-API
---
